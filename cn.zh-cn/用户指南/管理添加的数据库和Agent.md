# 管理添加的数据库和Agent<a name="dbss_01_0198"></a>

成功添加数据库后，您可以查看数据库信息、关闭、删除数据库。如果数据库添加了Agent，您还可以查看Agent信息、关闭或删除Agent。

## 前提条件<a name="section2707853181313"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   已成功添加数据库。
-   关闭数据库前，请确认数据库的“审计状态“为“已开启“。

## 查看数据库信息<a name="section1128063120241"></a>

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  进入数据库列表入口，如[图1](#dbss_01_0322_zh-cn_topic_0144723368_fig4155162273613)所示。

    **图 1**  进入数据库列表入口<a name="dbss_01_0322_zh-cn_topic_0144723368_fig4155162273613"></a>  
    ![](figures/进入数据库列表入口.png "进入数据库列表入口")

3.  在“选择实例“下拉列表框中，选择查看的数据库所属的实例。
4.  查看数据库信息，如[图2](#fig315603514243)所示，相关参数说明如[表1](#table4295843716304)所示。

    **图 2**  查看数据库和Agent信息<a name="fig315603514243"></a>  
    ![](figures/查看数据库和Agent信息.png "查看数据库和Agent信息")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >在列表右上方“全部审计状态“下拉列表框中选择数据库的审计状态，或输入数据库的关键字，可以搜索指定的数据库。

    **表 1**  数据库信息参数说明

    <a name="table4295843716304"></a>
    <table><thead align="left"><tr id="row4338993216304"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1"><p id="p2492361616304"><a name="p2492361616304"></a><a name="p2492361616304"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="61%" id="mcps1.2.4.1.2"><p id="p554697916304"><a name="p554697916304"></a><a name="p554697916304"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.3"><p id="p4665219216304"><a name="p4665219216304"></a><a name="p4665219216304"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row8736194992614"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p27371849182610"><a name="p27371849182610"></a><a name="p27371849182610"></a>数据库信息</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p673724912620"><a name="p673724912620"></a><a name="p673724912620"></a>数据库的名称、类型以及版本信息。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p1373734915267"><a name="p1373734915267"></a><a name="p1373734915267"></a>-</p>
    </td>
    </tr>
    <tr id="row8267640105117"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p137931346135116"><a name="p137931346135116"></a><a name="p137931346135116"></a>选择字符集</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p5793204619512"><a name="p5793204619512"></a><a name="p5793204619512"></a>数据库的编码字符集。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p1779314615513"><a name="p1779314615513"></a><a name="p1779314615513"></a>UTF8</p>
    </td>
    </tr>
    <tr id="row121453182104"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p8145151818109"><a name="p8145151818109"></a><a name="p8145151818109"></a>IP地址/端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p21451918111019"><a name="p21451918111019"></a><a name="p21451918111019"></a>数据库的IP地址。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p2145418161020"><a name="p2145418161020"></a><a name="p2145418161020"></a>192.168.0.0</p>
    <p id="p5775195515118"><a name="p5775195515118"></a><a name="p5775195515118"></a>3306</p>
    </td>
    </tr>
    <tr id="row0860165713317"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p12331342414"><a name="p12331342414"></a><a name="p12331342414"></a>实例名</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p17861057634"><a name="p17861057634"></a><a name="p17861057634"></a>数据库的实例名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p198613573313"><a name="p198613573313"></a><a name="p198613573313"></a>test</p>
    </td>
    </tr>
    <tr id="row1319658616304"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p6229055916304"><a name="p6229055916304"></a><a name="p6229055916304"></a>操作系统</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p1237050416304"><a name="p1237050416304"></a><a name="p1237050416304"></a>数据库运行的操作系统。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p1626715042213"><a name="p1626715042213"></a><a name="p1626715042213"></a>LINUX64</p>
    </td>
    </tr>
    <tr id="row091816547102"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p1918135431014"><a name="p1918135431014"></a><a name="p1918135431014"></a>审计状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p10918155441015"><a name="p10918155441015"></a><a name="p10918155441015"></a>数据库的审计状态，包括：</p>
    <a name="ul3352161171210"></a><a name="ul3352161171210"></a><ul id="ul3352161171210"><li>已开启</li><li>已关闭</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p179181854101013"><a name="p179181854101013"></a><a name="p179181854101013"></a>已开启</p>
    </td>
    </tr>
    <tr id="row1085198131115"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p16850815113"><a name="p16850815113"></a><a name="p16850815113"></a>Agent</p>
    </td>
    <td class="cellrowborder" valign="top" width="61%" headers="mcps1.2.4.1.2 "><p id="p986138101113"><a name="p986138101113"></a><a name="p986138101113"></a>单击<span class="uicontrol" id="uicontrol5612834181118"><a name="uicontrol5612834181118"></a><a name="uicontrol5612834181118"></a>“添加Agent”</span>，可以为数据库添加Agent。</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.3 "><p id="p5867861119"><a name="p5867861119"></a><a name="p5867861119"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >您可以根据使用需求，对添加的数据库执行以下操作：
    >-   关闭
    >    -   在需要关闭的数据库所在行的“操作“列，单击“关闭“后，在弹出的提示框中，单击“确定“，数据库的“审计状态“为“已关闭“。
    >    -   关闭数据库后，数据库安全审计将停止对该数据库进行安全审计。
    >-   删除
    >    -   在需要删除的数据库所在行的“操作“列，单击“删除“后，在弹出的提示框中，单击“确定“，删除该数据库。
    >    -   删除数据库后，如果需要对该数据库进行安全审计，请重新添加该数据库。


## 查看Agent信息<a name="section17294193018518"></a>

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  进入数据库列表入口，如[图3](#dbss_01_0322_zh-cn_topic_0144723368_fig4155162273613_1)所示。

    **图 3**  进入数据库列表入口<a name="dbss_01_0322_zh-cn_topic_0144723368_fig4155162273613_1"></a>  
    ![](figures/进入数据库列表入口.png "进入数据库列表入口")

3.  单击数据库左侧的![](figures/icon-drop.png)展开Agent的详细信息，如[图4](#fig1280134145116)所示，相关参数说明如[表2](#table146922503232)所示。

    **图 4**  查看数据库和Agent信息<a name="fig1280134145116"></a>  
    ![](figures/查看数据库和Agent信息.png "查看数据库和Agent信息")

    **表 2**  Agent参数说明

    <a name="table146922503232"></a>
    <table><thead align="left"><tr id="row369365019232"><th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.3.1.1"><p id="p1869325015239"><a name="p1869325015239"></a><a name="p1869325015239"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.39%" id="mcps1.2.3.1.2"><p id="p1069315072310"><a name="p1069315072310"></a><a name="p1069315072310"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row6693115010235"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p0693145011230"><a name="p0693145011230"></a><a name="p0693145011230"></a>Agent ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p88501519317"><a name="p88501519317"></a><a name="p88501519317"></a>Agent的ID，由系统自动生成。</p>
    </td>
    </tr>
    <tr id="row12694175032314"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p76945501231"><a name="p76945501231"></a><a name="p76945501231"></a>安装节点类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p631019101737"><a name="p631019101737"></a><a name="p631019101737"></a>安装节点的类型，包括<span class="parmvalue" id="parmvalue1537018312413"><a name="parmvalue1537018312413"></a><a name="parmvalue1537018312413"></a>“数据库端”</span>或<span class="parmvalue" id="parmvalue1580113340420"><a name="parmvalue1580113340420"></a><a name="parmvalue1580113340420"></a>“应用端”</span>。</p>
    </td>
    </tr>
    <tr id="row14693142715371"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p1869422718373"><a name="p1869422718373"></a><a name="p1869422718373"></a>安装节点IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p1544594615392"><a name="p1544594615392"></a><a name="p1544594615392"></a>安装Agent的节点的IP地址。</p>
    </td>
    </tr>
    <tr id="row364194913598"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p20641249185919"><a name="p20641249185919"></a><a name="p20641249185919"></a>操作系统</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p06424975911"><a name="p06424975911"></a><a name="p06424975911"></a>安装Agent运行的操作系统。</p>
    </td>
    </tr>
    <tr id="row06233118374"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p362131103717"><a name="p362131103717"></a><a name="p362131103717"></a>审计网卡名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p478844114409"><a name="p478844114409"></a><a name="p478844114409"></a>安装节点的网卡名称。</p>
    </td>
    </tr>
    <tr id="row246482404017"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p1646411249407"><a name="p1646411249407"></a><a name="p1646411249407"></a>CPU阈值(%)</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p1454215644116"><a name="p1454215644116"></a><a name="p1454215644116"></a>安装节点的CPU阈值，缺省值为<span class="parmvalue" id="parmvalue18165161114317"><a name="parmvalue18165161114317"></a><a name="parmvalue18165161114317"></a>“80”</span>。</p>
    </td>
    </tr>
    <tr id="row14911327164010"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p18492172774016"><a name="p18492172774016"></a><a name="p18492172774016"></a>内存阈值(%)</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p2073551313415"><a name="p2073551313415"></a><a name="p2073551313415"></a>安装节点的内存阈值，缺省值为<span class="parmvalue" id="parmvalue11322142320434"><a name="parmvalue11322142320434"></a><a name="parmvalue11322142320434"></a>“80”</span>。</p>
    </td>
    </tr>
    <tr id="row19965942805"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p1496574211014"><a name="p1496574211014"></a><a name="p1496574211014"></a>通用</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p6965642302"><a name="p6965642302"></a><a name="p6965642302"></a>Agent是否为通用Agent。</p>
    <p id="p690912171513"><a name="p690912171513"></a><a name="p690912171513"></a>否：需要用户下载Agent，并在<span class="parmvalue" id="parmvalue11214542113"><a name="parmvalue11214542113"></a><a name="parmvalue11214542113"></a>“数据库端”</span>或<span class="parmvalue" id="parmvalue15215114210110"><a name="parmvalue15215114210110"></a><a name="parmvalue15215114210110"></a>“应用端”</span>安装Agent。</p>
    <p id="p1572452285910"><a name="p1572452285910"></a><a name="p1572452285910"></a>是：不需要用户手动进行安装Agent。</p>
    </td>
    </tr>
    <tr id="row116912045932"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p166915454317"><a name="p166915454317"></a><a name="p166915454317"></a>运行状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p176911345637"><a name="p176911345637"></a><a name="p176911345637"></a>安装节点的运行状态。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >您可以根据使用需求，对添加的Agent执行以下操作：
    >-   关闭
    >    -   在需要关闭的Agent所在行的“操作“列，单击“关闭“后，在弹出的提示框中，单击“确定“，Agent状态为“关闭“。
    >    -   关闭Agent后，数据库安全审计将停止对连接该Agent的数据库进行安全审计。
    >-   删除
    >    -   在需要删除的Agent所在行的“操作“列，单击“删除“后，在弹出的提示框中，单击“确定“，删除该Agent。
    >    -   删除Agent后，如果需要对连接该Agent的数据库进行安全审计，请重新添加Agent。


