# 步骤二：添加Agent<a name="dbss_01_0188"></a>

将待审计数据库添加至数据库安全审计实例后，您需要根据您在云上实际部署的数据库选择添加Agent的方式以及在应用端或数据库端安装Agent。Agent程序会获取访问数据库流量、将流量数据上传到审计系统、接收审计系统配置命令和上报数据库状态监控数据，帮助您实现对数据库的安全审计。

完成添加Agent后，您还需要为Agent安装节点所在的安全组添加入方向规则TCP协议（8000端口）和UDP协议（7000-7100端口），使Agent与审计实例之间的网络连通，数据库安全审计才能对添加的数据库进行审计。

## 前提条件<a name="section070891116319"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   已成功添加数据库。

## 常见场景<a name="section984415120154"></a>

请您根据数据库类型以及数据库部署场景，为待审计的数据库添加Agent。数据库常见的部署场景说明如下：

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


添加Agent方式的详细说明如[表1](#table218115952118)所示。

>![](public_sys-resources/icon-notice.gif) **须知：** 
>-   当您的应用和数据库（ECS/BMS自建数据库）都部署在同一个节点上时，Agent需在数据库端添加。
>-   数据库安全审计还支持批量部署流量采集Agent，针对大规模业务场景（容器化部署应用、数据库（RDS关系型数据库）数量大），能够显著提升产品配置的效率，降低配置的复杂度，减少运维人员的日常维护压力。详细操作步骤，请参见[容器化部署数据库安全审计Agent](https://support.huaweicloud.com/bestpractice-dbss/dbss_06_0007.html)。

**表 1**  添加Agent方式说明

<a name="table218115952118"></a>
<table><thead align="left"><tr id="row1528919594215"><th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.1"><p id="p1128935917212"><a name="p1128935917212"></a><a name="p1128935917212"></a>使用场景</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p828913593219"><a name="p828913593219"></a><a name="p828913593219"></a>Agent安装节点</p>
</th>
<th class="cellrowborder" valign="top" width="29.587041295870414%" id="mcps1.2.5.1.3"><p id="p62896599219"><a name="p62896599219"></a><a name="p62896599219"></a>审计功能说明</p>
</th>
<th class="cellrowborder" valign="top" width="38.77612238776123%" id="mcps1.2.5.1.4"><p id="p9290205952117"><a name="p9290205952117"></a><a name="p9290205952117"></a>注意事项</p>
</th>
</tr>
</thead>
<tbody><tr id="row1329085922110"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p20290175916215"><a name="p20290175916215"></a><a name="p20290175916215"></a>ECS/BMS自建数据库</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p1629095932111"><a name="p1629095932111"></a><a name="p1629095932111"></a>数据库端</p>
</td>
<td class="cellrowborder" valign="top" width="29.587041295870414%" headers="mcps1.2.5.1.3 "><p id="p1529018598214"><a name="p1529018598214"></a><a name="p1529018598214"></a>可以审计所有访问该数据库的应用端的所有访问记录。</p>
</td>
<td class="cellrowborder" valign="top" width="38.77612238776123%" headers="mcps1.2.5.1.4 "><a name="ul1629035972114"></a><a name="ul1629035972114"></a><ul id="ul1629035972114"><li>在数据库端添加Agent。</li><li>当某个应用端连接多个ECS/BMS自建数据库时，所有连接该应用端的数据库都需要添加Agent。</li></ul>
</td>
</tr>
<tr id="row429015919219"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p1029055912111"><a name="p1029055912111"></a><a name="p1029055912111"></a>RDS关系型数据库</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p3290145932120"><a name="p3290145932120"></a><a name="p3290145932120"></a>应用端</p>
<p id="p104455011232"><a name="p104455011232"></a><a name="p104455011232"></a>（应用端部署在云上）</p>
</td>
<td class="cellrowborder" valign="top" width="29.587041295870414%" headers="mcps1.2.5.1.3 "><p id="p429035913213"><a name="p429035913213"></a><a name="p429035913213"></a>可以审计该应用端与其连接的所有数据库的访问记录。</p>
</td>
<td class="cellrowborder" valign="top" width="38.77612238776123%" headers="mcps1.2.5.1.4 "><a name="ul1429005916219"></a><a name="ul1429005916219"></a><ul id="ul1429005916219"><li>在应用端添加Agent。</li><li>当某个应用端连接多个RDS时，所有连接该应用端的RDS关系型数据库都需要添加Agent。当其中一个RDS选择<span class="parmname" id="parmname20164124182217"><a name="parmname20164124182217"></a><a name="parmname20164124182217"></a>“安装节点类型”</span>后，其余RDS添加Agent时，选择<span class="parmname" id="parmname1066911505229"><a name="parmname1066911505229"></a><a name="parmname1066911505229"></a>“选择已有Agent”</span>添加方式。详细操作请参见<a href="#li17692165032313">•“添加方式”选择“选择已有Agent”</a></li><li>当多个应用端连接同一个RDS时，所有连接该RDS的应用端都需要添加Agent。</li></ul>
</td>
</tr>
<tr id="row01451041229"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.1 "><p id="p91462482214"><a name="p91462482214"></a><a name="p91462482214"></a>RDS关系型数据库</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p57321338145019"><a name="p57321338145019"></a><a name="p57321338145019"></a>代理端（应用端部署在云下）</p>
</td>
<td class="cellrowborder" valign="top" width="29.587041295870414%" headers="mcps1.2.5.1.3 "><p id="p07324384506"><a name="p07324384506"></a><a name="p07324384506"></a>只能审计代理端与后端数据库之间的访问记录，无法审计应用端与后端数据库的访问记录。</p>
</td>
<td class="cellrowborder" valign="top" width="38.77612238776123%" headers="mcps1.2.5.1.4 "><a name="ul2118820252"></a><a name="ul2118820252"></a><ul id="ul2118820252"><li>在应用端添加Agent。</li><li><span class="parmname" id="parmname12632205416245"><a name="parmname12632205416245"></a><a name="parmname12632205416245"></a>“安装节点IP”</span>需要配置为代理端的IP地址。</li></ul>
</td>
</tr>
</tbody>
</table>

## 添加Agent（ECS/BMS自建数据库）<a name="section12371548164712"></a>

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  在页面上方选择“区域“后，单击页面左上方的![](figures/icon-list-1.png)，选择“安全与合规  \>  数据库安全服务“，进入数据库安全审计“总览“界面。
3.  在左侧导航树中，选择“数据库列表“，进入数据库列表界面。
4.  在“选择实例“下拉列表框中，选择需要添加Agent的数据库所属的实例。
5.  在添加的数据库所在行的“Agent“列，单击“添加Agent“。
6.  在弹出的“添加Agent“对话框中，选择添加方式，如[图5](#fig12967192134812)所示，相关参数说明如[表2](#table1996772134818)所示。

    **图 5**  在数据库端添加Agent<a name="fig12967192134812"></a>  
    ![](figures/在数据库端添加Agent.png "在数据库端添加Agent")

    **表 2**  添加Agent参数说明（ECS/BMS自建数据库）

    <a name="table1996772134818"></a>
    <table><thead align="left"><tr id="row17968122104812"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1"><p id="p1096817212485"><a name="p1096817212485"></a><a name="p1096817212485"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="61%" id="mcps1.2.4.1.2"><p id="p119682264813"><a name="p119682264813"></a><a name="p119682264813"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.3"><p id="p5968132124819"><a name="p5968132124819"></a><a name="p5968132124819"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14968162144818"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p39681213483"><a name="p39681213483"></a><a name="p39681213483"></a>添加方式</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><div class="p" id="p896882144810"><a name="p896882144810"></a><a name="p896882144810"></a>您可以选择Agent的添加方式。<a name="ul169686224815"></a><a name="ul169686224815"></a><ul id="ul169686224815"><li>选择已有Agent<p id="p29682021486"><a name="p29682021486"></a><a name="p29682021486"></a>当某个应用端连接了多个数据库时，如果该应用端的一个数据库已经在应用端添加了Agent。其他数据库在添加Agent时，只需要选择<span class="parmvalue" id="zh-cn_topic_0198815234_parmvalue19921182012126"><a name="zh-cn_topic_0198815234_parmvalue19921182012126"></a><a name="zh-cn_topic_0198815234_parmvalue19921182012126"></a>“选择已有Agent”</span>添加方式。</p>
    </li><li>创建Agent<p id="p89687234813"><a name="p89687234813"></a><a name="p89687234813"></a>如果待添加Agent的数据库需要创建Agent，请创建新的Agent。</p>
    </li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p17290203811"><a name="p17290203811"></a><a name="p17290203811"></a>创建Agent</p>
    </td>
    </tr>
    <tr id="row109705234815"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p597020211485"><a name="p597020211485"></a><a name="p597020211485"></a>安装节点类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p99701725487"><a name="p99701725487"></a><a name="p99701725487"></a>当<span class="parmname" id="parmname297062194815"><a name="parmname297062194815"></a><a name="parmname297062194815"></a>“添加方式”</span>选择<span class="parmvalue" id="parmvalue6970223486"><a name="parmvalue6970223486"></a><a name="parmvalue6970223486"></a>“创建Agent”</span>时，需配置该参数。</p>
    <p id="p397014213487"><a name="p397014213487"></a><a name="p397014213487"></a>审计ECS/BMS自建数据库，选择<span class="parmvalue" id="parmvalue5340204231111"><a name="parmvalue5340204231111"></a><a name="parmvalue5340204231111"></a>“数据库端”</span>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p7970192114813"><a name="p7970192114813"></a><a name="p7970192114813"></a>数据库端</p>
    </td>
    </tr>
    <tr id="row1736057195215"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p1960715385016"><a name="p1960715385016"></a><a name="p1960715385016"></a>操作系统</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p1660715375015"><a name="p1660715375015"></a><a name="p1660715375015"></a>指待审计的数据库的操作系统，支持<span class="parmvalue" id="parmvalue16838112813512"><a name="parmvalue16838112813512"></a><a name="parmvalue16838112813512"></a>“LINUX64”</span>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p156088533508"><a name="p156088533508"></a><a name="p156088533508"></a>LINUX64</p>
    <p id="p13799415141519"><a name="p13799415141519"></a><a name="p13799415141519"></a></p>
    </td>
    </tr>
    <tr id="row1252472714611"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p49040343244"><a name="p49040343244"></a><a name="p49040343244"></a>CPU阈值(%)</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p1290433416242"><a name="p1290433416242"></a><a name="p1290433416242"></a>可选参数。<span class="parmname" id="parmname2905734102411"><a name="parmname2905734102411"></a><a name="parmname2905734102411"></a>“安装节点类型”</span>选择<span class="parmvalue" id="parmvalue290543411243"><a name="parmvalue290543411243"></a><a name="parmvalue290543411243"></a>“应用端”</span>时，可以配置该参数。</p>
    <p id="p49051934192416"><a name="p49051934192416"></a><a name="p49051934192416"></a>指待审计的应用端节点的CPU阈值，缺省值为<span class="parmvalue" id="parmvalue590518346243"><a name="parmvalue590518346243"></a><a name="parmvalue590518346243"></a>“80”</span>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p1290511349244"><a name="p1290511349244"></a><a name="p1290511349244"></a>80</p>
    </td>
    </tr>
    <tr id="row58982331567"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p1190513411244"><a name="p1190513411244"></a><a name="p1190513411244"></a>内存阈值(%)</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p19905734182415"><a name="p19905734182415"></a><a name="p19905734182415"></a>可选参数。<span class="parmname" id="parmname1190503492416"><a name="parmname1190503492416"></a><a name="parmname1190503492416"></a>“安装节点类型”</span>选择<span class="parmvalue" id="parmvalue1990514349244"><a name="parmvalue1990514349244"></a><a name="parmvalue1990514349244"></a>“应用端”</span>时，可以配置该参数。</p>
    <p id="p1090513472410"><a name="p1090513472410"></a><a name="p1090513472410"></a>指待审计的应用端节点的内存阈值，缺省值为<span class="parmvalue" id="parmvalue5905143414242"><a name="parmvalue5905143414242"></a><a name="parmvalue5905143414242"></a>“80”</span>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p7905034182415"><a name="p7905034182415"></a><a name="p7905034182415"></a>80</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定“，Agent添加成功。
8.  单击数据库左侧的![](figures/icon-drop.png)展开该数据库的详细信息，查看添加的Agent信息，如[图6](#fig18975172124811)所示。

    **图 6**  Agent添加完成<a name="fig18975172124811"></a>  
    ![](figures/Agent添加完成.png "Agent添加完成")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >Agent添加完成后，请您确认添加的Agent信息正确。如果Agent添加不正确，请您在Agent所在行单击“删除“，删除Agent后，再重新添加Agent。


## 添加Agent（RDS关系型数据库）<a name="section1568164924617"></a>

当某个应用端连接了多个RDS时， 请按以下方式添加Agent：

-   连接该应用端所有的RDS都需要添加Agent。
-   如果连接该应用端的某个数据库已在应用端添加了Agent。其他数据库在添加Agent时，请选择“选择已有Agent“添加方式。

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  在页面上方选择“区域“后，单击页面左上方的![](figures/icon-list-1.png)，选择“安全与合规  \>  数据库安全服务“，进入数据库安全审计“总览“界面。
3.  在左侧导航树中，选择“数据库列表“，进入数据库列表界面。
4.  在“选择实例“下拉列表框中，选择需要添加Agent的数据库所属的实例。
5.  在添加的数据库所在行的“Agent“列，单击“添加Agent“。
6.  在弹出的“添加Agent“对话框中，选择添加方式，如[图7](#fig729959124017)和[图8](#fig9653154665)所示，相关参数说明如[表3](#table146922503232)所示。

    -   <a name="li17692165032313"></a>“添加方式“选择“选择已有Agent“

        在什么场景下需要选择“选择已有Agent“添加方式的详细介绍，请参见[在什么场景下需要选择“选择已有Agent”添加方式？](https://support.huaweicloud.com/dbss_faq/dbss_01_0286.html)。

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >选择“选择已有Agent“添加方式，如果您已在应用端安装了Agent，该数据库添加Agent后，数据库安全审计即可对该数据库进行审计。

        **图 7**  选择已有Agent<a name="fig729959124017"></a>  
        ![](figures/选择已有Agent.png "选择已有Agent")

    -   “添加方式“选择“创建Agent“

        如果待添加Agent的数据库需要创建Agent，请创建新的Agent。

        “安装节点类型“选择“应用端“，“安装节点IP“输入应用端内网IP地址。

        **图 8**  在应用端添加Agent<a name="fig9653154665"></a>  
        ![](figures/在应用端添加Agent.png "在应用端添加Agent")

    **表 3**  添加Agent参数说明（RDS关系型数据库）

    <a name="table146922503232"></a>
    <table><thead align="left"><tr id="row369365019232"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p1869325015239"><a name="p1869325015239"></a><a name="p1869325015239"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="61.01%" id="mcps1.2.4.1.2"><p id="p1069315072310"><a name="p1069315072310"></a><a name="p1069315072310"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.3"><p id="p136938501233"><a name="p136938501233"></a><a name="p136938501233"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row769315010235"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p6693145015238"><a name="p6693145015238"></a><a name="p6693145015238"></a>添加方式</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.01%" headers="mcps1.2.4.1.2 "><div class="p" id="p5693155082313"><a name="p5693155082313"></a><a name="p5693155082313"></a>您可以选择Agent的添加方式。<a name="dbss_01_0188_ul169686224815"></a><a name="dbss_01_0188_ul169686224815"></a><ul id="dbss_01_0188_ul169686224815"><li>选择已有Agent<p id="dbss_01_0188_p29682021486"><a name="dbss_01_0188_p29682021486"></a><a name="dbss_01_0188_p29682021486"></a>当某个应用端连接了多个数据库时，如果该应用端的一个数据库已经在应用端添加了Agent。其他数据库在添加Agent时，只需要选择<span class="parmvalue" id="dbss_01_0188_zh-cn_topic_0198815234_parmvalue19921182012126"><a name="dbss_01_0188_zh-cn_topic_0198815234_parmvalue19921182012126"></a><a name="dbss_01_0188_zh-cn_topic_0198815234_parmvalue19921182012126"></a>“选择已有Agent”</span>添加方式。</p>
    </li><li>创建Agent<p id="p510888134217"><a name="p510888134217"></a><a name="p510888134217"></a>如果待添加Agent的数据库需要创建Agent，请创建新的Agent。</p>
    </li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p5693155018234"><a name="p5693155018234"></a><a name="p5693155018234"></a>创建Agent</p>
    </td>
    </tr>
    <tr id="row12694175032314"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p76945501231"><a name="p76945501231"></a><a name="p76945501231"></a>安装节点类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.01%" headers="mcps1.2.4.1.2 "><p id="p6694155012231"><a name="p6694155012231"></a><a name="p6694155012231"></a>当<span class="parmname" id="dbss_01_0188_parmname297062194815"><a name="dbss_01_0188_parmname297062194815"></a><a name="dbss_01_0188_parmname297062194815"></a>“添加方式”</span>选择<span class="parmvalue" id="dbss_01_0188_parmvalue6970223486"><a name="dbss_01_0188_parmvalue6970223486"></a><a name="dbss_01_0188_parmvalue6970223486"></a>“创建Agent”</span>时，需配置该参数。</p>
    <p id="p769418506231"><a name="p769418506231"></a><a name="p769418506231"></a>审计RDS关系型数据库，需要选择<span class="parmvalue" id="parmvalue1769495019232"><a name="parmvalue1769495019232"></a><a name="parmvalue1769495019232"></a>“应用端”</span>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p18694135052320"><a name="p18694135052320"></a><a name="p18694135052320"></a>应用端</p>
    </td>
    </tr>
    <tr id="row14693142715371"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p1869422718373"><a name="p1869422718373"></a><a name="p1869422718373"></a>安装节点IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.01%" headers="mcps1.2.4.1.2 "><p id="p104441546163913"><a name="p104441546163913"></a><a name="p104441546163913"></a><span class="parmname" id="parmname87841450973"><a name="parmname87841450973"></a><a name="parmname87841450973"></a>“安装节点类型”</span>选择<span class="parmvalue" id="parmvalue127471541081"><a name="parmvalue127471541081"></a><a name="parmvalue127471541081"></a>“应用端”</span>时，需配置该参数。</p>
    <p id="p18043411752"><a name="p18043411752"></a><a name="p18043411752"></a>IP地址为应用端内网IP地址。</p>
    <p id="p5231578394"><a name="p5231578394"></a><a name="p5231578394"></a>IP地址支持IPv4（例如，192.168.1.1）和IPv6（例如，1050:0:0:0:5:600:300c:326b）格式。</p>
    <div class="notice" id="note1848771716436"><a name="note1848771716436"></a><a name="note1848771716436"></a><span class="noticetitle"> 须知： </span><div class="noticebody"><p id="p19161433104312"><a name="p19161433104312"></a><a name="p19161433104312"></a>当审计RDS关系型数据库且应用端在云下时，代理端将作为应用端，此时，<span class="parmname" id="parmname1560465312211"><a name="parmname1560465312211"></a><a name="parmname1560465312211"></a>“安装节点IP”</span>需要配置为代理端的IP地址。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p1569452710374"><a name="p1569452710374"></a><a name="p1569452710374"></a>192.168.1.1</p>
    </td>
    </tr>
    <tr id="row06233118374"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p362131103717"><a name="p362131103717"></a><a name="p362131103717"></a>审计网卡名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.01%" headers="mcps1.2.4.1.2 "><p id="p2788134164016"><a name="p2788134164016"></a><a name="p2788134164016"></a>可选参数。<span class="parmname" id="parmname1896692617818"><a name="parmname1896692617818"></a><a name="parmname1896692617818"></a>“安装节点类型”</span>选择<span class="parmvalue" id="parmvalue149661626385"><a name="parmvalue149661626385"></a><a name="parmvalue149661626385"></a>“应用端”</span>时，可以配置该参数。</p>
    <p id="p478844114409"><a name="p478844114409"></a><a name="p478844114409"></a>指待审计的应用端节点的网卡名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p1862183113717"><a name="p1862183113717"></a><a name="p1862183113717"></a>-</p>
    </td>
    </tr>
    <tr id="row246482404017"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p1646411249407"><a name="p1646411249407"></a><a name="p1646411249407"></a>CPU阈值(%)</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.01%" headers="mcps1.2.4.1.2 "><p id="p115421768411"><a name="p115421768411"></a><a name="p115421768411"></a>可选参数。<span class="parmname" id="parmname1734984517812"><a name="parmname1734984517812"></a><a name="parmname1734984517812"></a>“安装节点类型”</span>选择<span class="parmvalue" id="parmvalue134916451082"><a name="parmvalue134916451082"></a><a name="parmvalue134916451082"></a>“应用端”</span>时，可以配置该参数。</p>
    <p id="p1454215644116"><a name="p1454215644116"></a><a name="p1454215644116"></a>指待审计的应用端节点的CPU阈值，缺省值为<span class="parmvalue" id="parmvalue18165161114317"><a name="parmvalue18165161114317"></a><a name="parmvalue18165161114317"></a>“80”</span>。</p>
    <div class="notice" id="note1820183335018"><a name="note1820183335018"></a><a name="note1820183335018"></a><span class="noticetitle"> 须知： </span><div class="noticebody"><p id="p11820033115011"><a name="p11820033115011"></a><a name="p11820033115011"></a>当服务器的CPU超过设置的阈值，为了保证您业务的正常运行，Agent将自动关闭，停止运行。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p6464224104012"><a name="p6464224104012"></a><a name="p6464224104012"></a>80</p>
    </td>
    </tr>
    <tr id="row14911327164010"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p18492172774016"><a name="p18492172774016"></a><a name="p18492172774016"></a>内存阈值(%)</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.01%" headers="mcps1.2.4.1.2 "><p id="p3734613164114"><a name="p3734613164114"></a><a name="p3734613164114"></a>可选参数。<span class="parmname" id="parmname10159155016810"><a name="parmname10159155016810"></a><a name="parmname10159155016810"></a>“安装节点类型”</span>选择<span class="parmvalue" id="parmvalue121595501780"><a name="parmvalue121595501780"></a><a name="parmvalue121595501780"></a>“应用端”</span>时，可以配置该参数。</p>
    <p id="p2073551313415"><a name="p2073551313415"></a><a name="p2073551313415"></a>指待审计的应用端节点的内存阈值，缺省值为<span class="parmvalue" id="parmvalue11322142320434"><a name="parmvalue11322142320434"></a><a name="parmvalue11322142320434"></a>“80”</span>。</p>
    <div class="notice" id="note106851122105215"><a name="note106851122105215"></a><a name="note106851122105215"></a><span class="noticetitle"> 须知： </span><div class="noticebody"><p id="p46858221526"><a name="p46858221526"></a><a name="p46858221526"></a>当服务器上的内存超过设置的阈值，为了保证您业务的正常运行，Agent将自动关闭，停止运行。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p84921627194013"><a name="p84921627194013"></a><a name="p84921627194013"></a>80</p>
    </td>
    </tr>
    <tr id="row19648105334818"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p7649135319487"><a name="p7649135319487"></a><a name="p7649135319487"></a>操作系统</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.01%" headers="mcps1.2.4.1.2 "><p id="p16501353154818"><a name="p16501353154818"></a><a name="p16501353154818"></a>可选参数。<span class="parmname" id="parmname12206171714917"><a name="parmname12206171714917"></a><a name="parmname12206171714917"></a>“安装节点类型”</span>选择<span class="parmvalue" id="parmvalue820641713497"><a name="parmvalue820641713497"></a><a name="parmvalue820641713497"></a>“应用端”</span>时，可以配置该参数。</p>
    <p id="p1651413195494"><a name="p1651413195494"></a><a name="p1651413195494"></a>指待审计的应用端节点的操作系统，可以选择<span class="parmvalue" id="parmvalue61112313505"><a name="parmvalue61112313505"></a><a name="parmvalue61112313505"></a>“LINUX64”</span>或<span class="parmvalue" id="parmvalue044843717504"><a name="parmvalue044843717504"></a><a name="parmvalue044843717504"></a>“WINDOWS64”</span>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p1665018536487"><a name="p1665018536487"></a><a name="p1665018536487"></a>LINUX64</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定“，Agent添加成功。
8.  单击数据库左侧的![](figures/icon-drop.png)展开该数据库的详细信息，查看添加的Agent信息，如[图9](#fig1470611221310)所示。

    **图 9**  Agent已添加完成<a name="fig1470611221310"></a>  
    ![](figures/Agent已添加完成.png "Agent已添加完成")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >Agent添加完成后，请您确认添加的Agent信息正确。如果Agent添加不正确，请您在Agent所在行单击“删除“，删除Agent后，再重新添加Agent。


## 后续处理<a name="section11581123681920"></a>

Agent添加完成后，您还需要为数据库安全审计实例所在的安全组添加入方向规则TCP协议（8000端口）和UDP协议（7000-7100端口），使Agent与审计实例之间的网络连通，数据库安全审计才能对添加的数据库进行审计。有关添加安全组规则的详细操作，请参见[添加安全组规则](步骤三-添加安全组规则.md)。

