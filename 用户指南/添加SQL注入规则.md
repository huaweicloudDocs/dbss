# 添加SQL注入规则<a name="dbss_01_0362"></a>

数据库安全审计提供“添加SQL注入规则“，您可根据需要自定义添加对应的SQL规则，添加后可以对成功连接数据库安全审计的所有数据进行安全审计。

## 前提条件<a name="section070891116319"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   已成功添加数据库并开启审计功能。
-   已成功添加数据库。

## 操作步骤<a name="section1828521219565"></a>

1.  [登录管理控制台](https://auth.huaweicloud.com/authui/login.html?service=https%3A%2F%2Fconsole.huaweicloud.com%2Fconsole%2F#/login)。
2.  在页面上方选择“区域“后，单击页面左上方的![](figures/icon-list-1.png)，选择“安全与合规  \>  数据库安全服务“，进入数据库安全审计“总览“界面。
3.  在左侧导航树中，选择“审计规则“。
4.  在“选择实例“下拉列表框中，选择需要添加审计范围的实例。
5.  选择“SQL注入“页签。
6.  单击“添加SQL注入规则“，在弹窗中填写相关信息，如[图1](#fig348598171219)所示，参数说明如[表1](#table448716810124)所示。

    **图 1**  添加SQL注入规则<a name="fig348598171219"></a>  
    ![](figures/添加SQL注入规则.png "添加SQL注入规则")

    **表 1**  SQL注入规则参数说明

    <a name="table448716810124"></a>
    <table><thead align="left"><tr id="dbss_01_0191_row27104486104"><th class="cellrowborder" valign="top" width="14.431443144314432%" id="mcps1.2.4.1.1"><p id="dbss_01_0191_p1710104815102"><a name="dbss_01_0191_p1710104815102"></a><a name="dbss_01_0191_p1710104815102"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.235223522352236%" id="mcps1.2.4.1.2"><p id="dbss_01_0191_p1671054861012"><a name="dbss_01_0191_p1671054861012"></a><a name="dbss_01_0191_p1671054861012"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="dbss_01_0191_p37101448201010"><a name="dbss_01_0191_p37101448201010"></a><a name="dbss_01_0191_p37101448201010"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dbss_01_0191_row1710748151012"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="dbss_01_0191_p12710114815102"><a name="dbss_01_0191_p12710114815102"></a><a name="dbss_01_0191_p12710114815102"></a>规则名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="dbss_01_0191_p571084815102"><a name="dbss_01_0191_p571084815102"></a><a name="dbss_01_0191_p571084815102"></a>目标SQL规则的名称，可自定义输入。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="dbss_01_0191_p167107484102"><a name="dbss_01_0191_p167107484102"></a><a name="dbss_01_0191_p167107484102"></a>邮编SQL注入规则</p>
    </td>
    </tr>
    <tr id="dbss_01_0191_row57101948191017"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="dbss_01_0191_p1971084811015"><a name="dbss_01_0191_p1971084811015"></a><a name="dbss_01_0191_p1971084811015"></a>风险等级</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="dbss_01_0191_p6040559116304"><a name="dbss_01_0191_p6040559116304"></a><a name="dbss_01_0191_p6040559116304"></a>目标SQL规则的风险级别，可以选择以下级别：</p>
    <a name="dbss_01_0191_ul155751241152314"></a><a name="dbss_01_0191_ul155751241152314"></a><ul id="dbss_01_0191_ul155751241152314"><li>高</li><li>中</li><li>低</li><li>无风险</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="dbss_01_0191_p3710134812101"><a name="dbss_01_0191_p3710134812101"></a><a name="dbss_01_0191_p3710134812101"></a>中</p>
    </td>
    </tr>
    <tr id="dbss_01_0191_row371084871016"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="dbss_01_0191_p2710124819109"><a name="dbss_01_0191_p2710124819109"></a><a name="dbss_01_0191_p2710124819109"></a>状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="dbss_01_0191_p153321841736"><a name="dbss_01_0191_p153321841736"></a><a name="dbss_01_0191_p153321841736"></a>开启或关闭当前SQL注入规则。</p>
    <a name="dbss_01_0191_ul934875119443"></a><a name="dbss_01_0191_ul934875119443"></a><ul id="dbss_01_0191_ul934875119443"><li><a name="dbss_01_0191_image7580817633"></a><a name="dbss_01_0191_image7580817633"></a><span><img id="dbss_01_0191_image7580817633" src="figures/icon-open-3.png"></span>：开启</li><li><a name="dbss_01_0191_image1439810311932"></a><a name="dbss_01_0191_image1439810311932"></a><span><img id="dbss_01_0191_image1439810311932" src="figures/icon-close-2.png"></span>：关闭</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="dbss_01_0191_p17710124881011"><a name="dbss_01_0191_p17710124881011"></a><a name="dbss_01_0191_p17710124881011"></a><a name="dbss_01_0191_image13111511191411"></a><a name="dbss_01_0191_image13111511191411"></a><span><img id="dbss_01_0191_image13111511191411" src="figures/icon-open-4.png"></span></p>
    </td>
    </tr>
    <tr id="dbss_01_0191_row1771094861019"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="dbss_01_0191_p9710154811108"><a name="dbss_01_0191_p9710154811108"></a><a name="dbss_01_0191_p9710154811108"></a>正则表达式</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="dbss_01_0191_p671074813103"><a name="dbss_01_0191_p671074813103"></a><a name="dbss_01_0191_p671074813103"></a>目标SQL规则采用正则表达式检测的公式，需要您根据需要检测的内容来输入确定。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="dbss_01_0191_p735111694316"><a name="dbss_01_0191_p735111694316"></a><a name="dbss_01_0191_p735111694316"></a>^\d{<span>6</span>}$</p>
    </td>
    </tr>
    <tr id="dbss_01_0191_row1271011485107"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="dbss_01_0191_p14710204861015"><a name="dbss_01_0191_p14710204861015"></a><a name="dbss_01_0191_p14710204861015"></a>原始数据</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="dbss_01_0191_p1661738172118"><a name="dbss_01_0191_p1661738172118"></a><a name="dbss_01_0191_p1661738172118"></a>正则表达式能检测的正确数据。</p>
    <p id="dbss_01_0191_p1471012487105"><a name="dbss_01_0191_p1471012487105"></a><a name="dbss_01_0191_p1471012487105"></a>输入正则表达式能检测的正确数据，单击<span class="uicontrol" id="dbss_01_0191_uicontrol46492016162118"><a name="dbss_01_0191_uicontrol46492016162118"></a><a name="dbss_01_0191_uicontrol46492016162118"></a>“测试”</span>对正则表达式进行检测。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="dbss_01_0191_p7710448101018"><a name="dbss_01_0191_p7710448101018"></a><a name="dbss_01_0191_p7710448101018"></a>628307</p>
    </td>
    </tr>
    <tr id="dbss_01_0191_row1710164871010"><td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.4.1.1 "><p id="dbss_01_0191_p1710648131012"><a name="dbss_01_0191_p1710648131012"></a><a name="dbss_01_0191_p1710648131012"></a>结果</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.235223522352236%" headers="mcps1.2.4.1.2 "><p id="dbss_01_0191_p588013323212"><a name="dbss_01_0191_p588013323212"></a><a name="dbss_01_0191_p588013323212"></a>显示测试的结果：</p>
    <a name="dbss_01_0191_ul12565111265512"></a><a name="dbss_01_0191_ul12565111265512"></a><ul id="dbss_01_0191_ul12565111265512"><li>命中</li><li>未命中<div class="note" id="dbss_01_0191_note168861814112310"><a name="dbss_01_0191_note168861814112310"></a><a name="dbss_01_0191_note168861814112310"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="dbss_01_0191_p10886714162318"><a name="dbss_01_0191_p10886714162318"></a><a name="dbss_01_0191_p10886714162318"></a>测试结果为<span class="wintitle" id="dbss_01_0191_wintitle91511057112415"><a name="dbss_01_0191_wintitle91511057112415"></a><a name="dbss_01_0191_wintitle91511057112415"></a>“命中”</span>：表示正则表达式无误；</p>
    <p id="dbss_01_0191_p20770152122418"><a name="dbss_01_0191_p20770152122418"></a><a name="dbss_01_0191_p20770152122418"></a>测试结果为<span class="wintitle" id="dbss_01_0191_wintitle87027534249"><a name="dbss_01_0191_wintitle87027534249"></a><a name="dbss_01_0191_wintitle87027534249"></a>“未命中”</span>：表示正则表达式有误。</p>
    </div></div>
    </li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="dbss_01_0191_p107101648171010"><a name="dbss_01_0191_p107101648171010"></a><a name="dbss_01_0191_p107101648171010"></a>命中</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  填写完成，确认信息无误，单击“确认“，添加完成，新增的SQL注入规则默认为SQL注入列表第一条。

