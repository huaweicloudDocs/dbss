# 启用或禁用SQL注入检测<a name="dbss_01_0191"></a>

数据库安全审计的SQL注入检测默认开启，您可以禁用或启用SQL注入的检测规则。

>![](public_sys-resources/icon-notice.gif) **须知：** 
>一条审计数据只能命中SQL注入检测中的一个规则。

## 前提条件<a name="section070891116319"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   SQL注入检测的状态为“已禁用“时，可以启用SQL注入检测。
-   SQL注入检测的状态为“已启用“时，可以禁用SQL注入检测。

## 禁用SQL注入检测<a name="section1466619111369"></a>

SQL注入检测默认开启，您可以根据使用需要禁用SQL注入检查规则。禁用SQL注入检测规则后，该审计规则在审计中将不生效。

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  在页面上方选择“区域“后，单击页面左上方的![](figures/icon-list-1.png)，选择“安全与合规  \>  数据库安全服务“，进入数据库安全审计“总览“界面。
3.  在左侧导航树中，选择“审计规则“。
4.  在“选择实例“下拉列表框中，选择需要禁用SQL注入检测的实例。
5.  选择“SQL注入“页签。
6.  在SQL注入检测规则所在行的“操作“列，单击“设置优先级“，在弹出的窗口中单击“优先级“的选框选择想要设置的优先等级，数字越小优先级越高，如[图1](#fig1937132125810)所示，选择完成，单击“确定”完成设置。

    **图 1**  设置优先级<a name="fig1937132125810"></a>  
    ![](figures/设置优先级.png "设置优先级")

7.  在SQL注入检测规则所在行的“操作“列，单击“禁用“，如[图2](#fig148017166466)所示。

    **图 2**  禁用SQL注入检测规则<a name="fig148017166466"></a>  
    ![](figures/禁用SQL注入检测规则.png "禁用SQL注入检测规则")

    禁用SQL注入检测成功，该SQL注入检测规则的状态为“已禁用“。

8.  单击“操作“列的“编辑“，可对目标规则的参数进行编辑，如[图3](#fig1448418914912)所示；参数说明如[表1](#table14709144861013)所示，编辑完成，确认信息无误，单击“确认“，完成修改。

    **图 3**  编辑SQL注入规则<a name="fig1448418914912"></a>  
    ![](figures/编辑SQL注入规则.png "编辑SQL注入规则")

    **表 1**  SQL注入规则参数说明

    <a name="table14709144861013"></a>
    <table><thead align="left"><tr id="row27104486104"><th class="cellrowborder" valign="top" width="14.431443144314432%" id="mcps1.2.4.1.1"><p id="p1710104815102"><a name="p1710104815102"></a><a name="p1710104815102"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.235223522352236%" id="mcps1.2.4.1.2"><p id="p1671054861012"><a name="p1671054861012"></a><a name="p1671054861012"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p37101448201010"><a name="p37101448201010"></a><a name="p37101448201010"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1710748151012"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="p12710114815102"><a name="p12710114815102"></a><a name="p12710114815102"></a>规则名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="p571084815102"><a name="p571084815102"></a><a name="p571084815102"></a>目标SQL规则的名称，可自定义输入。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p167107484102"><a name="p167107484102"></a><a name="p167107484102"></a>邮编SQL注入规则</p>
    </td>
    </tr>
    <tr id="row57101948191017"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="p1971084811015"><a name="p1971084811015"></a><a name="p1971084811015"></a>风险等级</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="p6040559116304"><a name="p6040559116304"></a><a name="p6040559116304"></a>目标SQL规则的风险级别，可以选择以下级别：</p>
    <a name="ul155751241152314"></a><a name="ul155751241152314"></a><ul id="ul155751241152314"><li>高</li><li>中</li><li>低</li><li>无风险</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p3710134812101"><a name="p3710134812101"></a><a name="p3710134812101"></a>中</p>
    </td>
    </tr>
    <tr id="row371084871016"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="p2710124819109"><a name="p2710124819109"></a><a name="p2710124819109"></a>状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="p153321841736"><a name="p153321841736"></a><a name="p153321841736"></a>开启或关闭当前SQL注入规则。</p>
    <a name="ul934875119443"></a><a name="ul934875119443"></a><ul id="ul934875119443"><li><a name="image7580817633"></a><a name="image7580817633"></a><span><img id="image7580817633" src="figures/icon-open-3.png"></span>：开启</li><li><a name="image1439810311932"></a><a name="image1439810311932"></a><span><img id="image1439810311932" src="figures/icon-close-2.png"></span>：关闭</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p17710124881011"><a name="p17710124881011"></a><a name="p17710124881011"></a><a name="image13111511191411"></a><a name="image13111511191411"></a><span><img id="image13111511191411" src="figures/icon-open-4.png"></span></p>
    </td>
    </tr>
    <tr id="row1771094861019"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="p9710154811108"><a name="p9710154811108"></a><a name="p9710154811108"></a>正则表达式</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="p671074813103"><a name="p671074813103"></a><a name="p671074813103"></a>目标SQL规则采用正则表达式检测的公式，需要您根据需要检测的内容来输入确定。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p735111694316"><a name="p735111694316"></a><a name="p735111694316"></a>^\d{<span>6</span>}$</p>
    </td>
    </tr>
    <tr id="row1271011485107"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="p14710204861015"><a name="p14710204861015"></a><a name="p14710204861015"></a>原始数据</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="p1661738172118"><a name="p1661738172118"></a><a name="p1661738172118"></a>正则表达式能检测的正确数据。</p>
    <p id="p1471012487105"><a name="p1471012487105"></a><a name="p1471012487105"></a>输入正则表达式能检测的正确数据，单击<span class="uicontrol" id="uicontrol46492016162118"><a name="uicontrol46492016162118"></a><a name="uicontrol46492016162118"></a>“测试”</span>对正则表达式进行检测。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p7710448101018"><a name="p7710448101018"></a><a name="p7710448101018"></a>628307</p>
    </td>
    </tr>
    <tr id="row1710164871010"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="p1710648131012"><a name="p1710648131012"></a><a name="p1710648131012"></a>结果</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="p588013323212"><a name="p588013323212"></a><a name="p588013323212"></a>显示测试的结果：</p>
    <a name="ul12565111265512"></a><a name="ul12565111265512"></a><ul id="ul12565111265512"><li>命中</li><li>未命中<div class="note" id="note168861814112310"><a name="note168861814112310"></a><a name="note168861814112310"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p10886714162318"><a name="p10886714162318"></a><a name="p10886714162318"></a>测试结果为<span class="wintitle" id="wintitle91511057112415"><a name="wintitle91511057112415"></a><a name="wintitle91511057112415"></a>“命中”</span>：表示正则表达式无误；</p>
    <p id="p20770152122418"><a name="p20770152122418"></a><a name="p20770152122418"></a>测试结果为<span class="wintitle" id="wintitle87027534249"><a name="wintitle87027534249"></a><a name="wintitle87027534249"></a>“未命中”</span>：表示正则表达式有误。</p>
    </div></div>
    </li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p107101648171010"><a name="p107101648171010"></a><a name="p107101648171010"></a>命中</p>
    </td>
    </tr>
    </tbody>
    </table>

9.  单击“操作“列的“删除“，对目标规则进行删除。

## 后续处理<a name="section116222113496"></a>

禁用SQL注入检测规则后，如果您需要启动该规则，请在SQL注入检测规则所在行的“操作“列，单击“启用“，如[图4](#fig185497132517)所示，启用该规则。

**图 4**  启用SQL注入检测规则<a name="fig185497132517"></a>  
![](figures/启用SQL注入检测规则.png "启用SQL注入检测规则")

启用SQL注入检测成功，该SQL注入检测规则的状态为“已启用“。

