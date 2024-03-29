# 安装Agent（Windows操作系统）<a name="dbss_01_0315"></a>

安装Agent后，你才能开启数据库安全审计。通过本节介绍，您将了解如何在Windows操作系统的节点上安装Agent。Linux操作系统的Agent安装请参见[安装Agent（Linux操作系统）](安装Agent（Linux操作系统）.md)。

## 前提条件<a name="section070891116319"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   数据库已成功添加Agent
-   已获取Windows操作系统Agent安装包。
-   安装Agent节点的运行系统满足Windows系统版本要求。有关Windows系统版本的要求，请参见[Agent可以安装在哪些Windows操作系统上？](https://support.huaweicloud.com/dbss_faq/dbss_01_0318.html)。

## 常见安装场景<a name="section672894812914"></a>

请您根据数据库的类型以及部署场景，在数据库端或应用端安装Agent。数据库常见的部署场景说明如下：

-   ECS/BMS自建数据库的常见部署场景如[图1](#dbss_01_0254_fig0617131314411)和[图2](#dbss_01_0254_fig1131385013914)所示。

    **图 1**  一个应用端连接多个ECS/BMS自建数据库<a name="dbss_01_0254_fig0617131314411"></a>  
    ![](figures/一个应用端连接多个ECS-BMS自建数据库.png "一个应用端连接多个ECS-BMS自建数据库")

    **图 2**  多个应用端连接同一个ECS/BMS自建数据库<a name="dbss_01_0254_fig1131385013914"></a>  
    ![](figures/多个应用端连接同一个ECS-BMS自建数据库.png "多个应用端连接同一个ECS-BMS自建数据库")

-   RDS关系型数据库的常见部署场景如[图3](#dbss_01_0254_fig76418538416)和[图4](#dbss_01_0254_fig766123541110)所示。

    **图 3**  一个应用端连接多个RDS<a name="dbss_01_0254_fig76418538416"></a>  
    ![](figures/一个应用端连接多个RDS.png "一个应用端连接多个RDS")

    **图 4**  多个应用端连接同一个RDS<a name="dbss_01_0254_fig766123541110"></a>  
    ![](figures/多个应用端连接同一个RDS.png "多个应用端连接同一个RDS")


安装Agent节点的详细说明如[表1](#dbss_01_0254_zh-cn_topic_0110856029_table4295843716304)所示。

>![](public_sys-resources/icon-notice.gif) **须知：** 
>当您的应用和数据库（ECS/BMS自建数据库）都部署在同一个节点上时，Agent需在数据库端安装。

**表 1**  安装Agent场景说明

<a name="dbss_01_0254_zh-cn_topic_0110856029_table4295843716304"></a>
<table><thead align="left"><tr id="dbss_01_0254_zh-cn_topic_0110856029_row4338993216304"><th class="cellrowborder" valign="top" width="16.91%" id="mcps1.2.5.1.1"><p id="dbss_01_0254_p242511529611"><a name="dbss_01_0254_p242511529611"></a><a name="dbss_01_0254_p242511529611"></a>使用场景</p>
</th>
<th class="cellrowborder" valign="top" width="15.61%" id="mcps1.2.5.1.2"><p id="dbss_01_0254_p669218115912"><a name="dbss_01_0254_p669218115912"></a><a name="dbss_01_0254_p669218115912"></a>Agent安装节点</p>
</th>
<th class="cellrowborder" valign="top" width="29.21%" id="mcps1.2.5.1.3"><p id="dbss_01_0254_zh-cn_topic_0110856029_p554697916304"><a name="dbss_01_0254_zh-cn_topic_0110856029_p554697916304"></a><a name="dbss_01_0254_zh-cn_topic_0110856029_p554697916304"></a>审计功能说明</p>
</th>
<th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.2.5.1.4"><p id="dbss_01_0254_p1457555517420"><a name="dbss_01_0254_p1457555517420"></a><a name="dbss_01_0254_p1457555517420"></a>注意事项</p>
</th>
</tr>
</thead>
<tbody><tr id="dbss_01_0254_zh-cn_topic_0110856029_row3896937416304"><td class="cellrowborder" valign="top" width="16.91%" headers="mcps1.2.5.1.1 "><p id="dbss_01_0254_p1742645217615"><a name="dbss_01_0254_p1742645217615"></a><a name="dbss_01_0254_p1742645217615"></a>ECS/BMS自建数据库</p>
</td>
<td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.2 "><p id="dbss_01_0254_p96937116596"><a name="dbss_01_0254_p96937116596"></a><a name="dbss_01_0254_p96937116596"></a>数据库端</p>
</td>
<td class="cellrowborder" valign="top" width="29.21%" headers="mcps1.2.5.1.3 "><p id="dbss_01_0254_p163512146517"><a name="dbss_01_0254_p163512146517"></a><a name="dbss_01_0254_p163512146517"></a>可以审计所有访问该数据库的应用端的所有访问记录。</p>
</td>
<td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.2.5.1.4 "><a name="dbss_01_0254_ul1434325082513"></a><a name="dbss_01_0254_ul1434325082513"></a><ul id="dbss_01_0254_ul1434325082513"><li>在数据库端安装Agent。</li><li>当某个应用端连接多个ECS/BMS自建数据库时，需要在所有连接该应用端的数据库端安装Agent。</li></ul>
</td>
</tr>
<tr id="dbss_01_0254_zh-cn_topic_0110856029_row1319658616304"><td class="cellrowborder" valign="top" width="16.91%" headers="mcps1.2.5.1.1 "><p id="dbss_01_0254_p10426195218611"><a name="dbss_01_0254_p10426195218611"></a><a name="dbss_01_0254_p10426195218611"></a>RDS关系型数据库</p>
</td>
<td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.2 "><p id="dbss_01_0254_p1669315145912"><a name="dbss_01_0254_p1669315145912"></a><a name="dbss_01_0254_p1669315145912"></a>应用端（应用端部署在云上）</p>
</td>
<td class="cellrowborder" valign="top" width="29.21%" headers="mcps1.2.5.1.3 "><p id="dbss_01_0254_p137861430175114"><a name="dbss_01_0254_p137861430175114"></a><a name="dbss_01_0254_p137861430175114"></a>可以审计该应用端与其连接的所有数据库的访问记录。</p>
</td>
<td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.2.5.1.4 "><a name="dbss_01_0254_ul832714025916"></a><a name="dbss_01_0254_ul832714025916"></a><ul id="dbss_01_0254_ul832714025916"><li>在应用端安装Agent。</li><li>当多个应用端连接同一个RDS时，所有连接该RDS的应用端都需要安装Agent。</li></ul>
</td>
</tr>
<tr id="dbss_01_0254_row673153818506"><td class="cellrowborder" valign="top" width="16.91%" headers="mcps1.2.5.1.1 "><p id="dbss_01_0254_p19307124313503"><a name="dbss_01_0254_p19307124313503"></a><a name="dbss_01_0254_p19307124313503"></a>RDS关系型数据库</p>
</td>
<td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.2 "><p id="dbss_01_0254_p57321338145019"><a name="dbss_01_0254_p57321338145019"></a><a name="dbss_01_0254_p57321338145019"></a>代理端（应用端部署在云下）</p>
</td>
<td class="cellrowborder" valign="top" width="29.21%" headers="mcps1.2.5.1.3 "><p id="dbss_01_0254_p07324384506"><a name="dbss_01_0254_p07324384506"></a><a name="dbss_01_0254_p07324384506"></a>只能审计代理端与后端数据库之间的访问记录，无法审计应用端与后端数据库的访问记录。</p>
</td>
<td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.2.5.1.4 "><p id="dbss_01_0254_p31819567512"><a name="dbss_01_0254_p31819567512"></a><a name="dbss_01_0254_p31819567512"></a>在代理端安装Agent。</p>
</td>
</tr>
</tbody>
</table>

## 安装Agent<a name="section1410916716365"></a>

1.  在Windows主机安装“Npcap“软件。
    -   如果该Windows主机已安装“Npcap“，请执行[2](#li536717914201)。
    -   如果该Windows主机未安装“Npcap“，请执行以下步骤：
        1.  请前往[https://nmap.org/npcap/](https://nmap.org/npcap/)下载Npcap最新软件安装包。

            **图 5**  下载npcap<a name="fig172365020285"></a>  
            ![](figures/下载npcap.png "下载npcap")

        2.  将下载好的npcap-_xxxx_.exe软件安装包上传至需要安装agent的虚拟机。
        3.  双击npcap软件安装包。
        4.  在弹出的对话框中，单击“I Agree“，如[图6](#fig114541164118)所示。

            **图 6**  同意安装“Npcap“<a name="fig114541164118"></a>  
            ![](figures/同意安装Npcap.png "同意安装Npcap")

        5.  在弹出的对话框中，单击“Install“，不勾选安装选项，如[图7](#fig124541516111114)所示。

            **图 7**  安装“Npcap“<a name="fig124541516111114"></a>  
            ![](figures/安装Npcap.png "安装Npcap")

        6.  在弹出的对话框中，单击“Next“。

            ![](figures/安装NPCAP-02.png)

        7.  单击“Finish“，完成安装。

            ![](figures/NPCAP安装完成.png)


2.  <a name="li536717914201"></a>以“Administrator“用户登录到Windows主机。
3.  将下载的Agent安装包“xxx.zip“复制到该主机任意一个目录下。
4.  进入Agent安装包所在目录，并解压缩安装包。
5.  进入解压后的文件夹，双击“install.bat“执行文件。
6.  安装成功，界面如[图8](#fig1160640132710)所示，按任意键结束安装。

    **图 8**  Agent安装成功<a name="fig1160640132710"></a>  
    ![](figures/Agent安装成功.png "Agent安装成功")

7.  安装完成后，在Windows任务管理器中查看“dbss\_audit\_agent“进程。

    如果进程不存在，说明Agent安装失败，请尝试重新安装Agent。


## 相关操作<a name="section3657198173220"></a>

-   有关添加Agent的详细操作，请参见[步骤二：添加Agent](步骤二-添加Agent.md)。
-   数据库开启SSL时，将不能使用数据库安全审计功能。如果您需要使用数据库安全审计功能，请关闭数据库的SSL。关闭数据库SSL的详细操作，请参见[如何关闭数据库SSL？](https://support.huaweicloud.com/dbss_faq/dbss_01_0283.html)。
-   有关卸载Agent的详细操作，请参见[卸载Agent](卸载Agent.md)。

