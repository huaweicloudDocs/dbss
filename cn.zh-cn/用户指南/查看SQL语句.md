# 查看SQL语句<a name="ZH-CN_TOPIC_0145057230"></a>

本章节介绍如何查看数据库安全审计的SQL语句信息。

## 前提条件<a name="section441811405410"></a>

-   已获取管理控制台的登录账号与密码。
-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   已开启数据库审计，并在数据库端或应用端成功安装Agent。
-   已成功设置审计规则。

## 操作步骤<a name="section16337113512514"></a>

1.  登录管理控制台。
2.  单击管理控制台左上角的![](figures/项目.png)，选择区域或项目。
3.  单击管理控制台上方的“服务列表“，选择“安全  \>  数据库安全服务 DBSS“，进入数据库安全防护实例列表界面。
4.  在左侧导航树中，选择“数据库安全服务  \>  数据库安全审计“，进入数据库安全审计实例列表界面。
5.  在数据库安全审计实例列表中，单击需要查看SQL语句的实例名称，如[图1](#fig99553501795)所示。

    **图 1**  数据库安全审计实例列表<a name="fig99553501795"></a>  
    ![](figures/数据库安全审计实例列表.png "数据库安全审计实例列表")

6.  在“实例详情“界面，单击“SQL语句“。
7.  查看SQL语句信息，如[图2](#fig1748292125513)所示，相关参数说明如[表1](#table4295843716304)所示。

    **图 2**  查看SQL语句<a name="fig1748292125513"></a>  
    ![](figures/查看SQL语句.png "查看SQL语句")

    您可以按照以下方法，查询指定的SQL语句。

    -   选择“时间“，或单击![](figures/日历-14.png)，选择开始时间和结束时间，单击“提交“，列表显示该时间段的SQL语句。
    -   选择“风险级别“，单击“提交“，列表显示该级别的SQL语句。
    -   单击“高级选项“后的![](figures/下拉.png)，输入相关信息，如[图3](#fig1208529493)所示，单击“提交“，列表显示该选项的SQL语句。

        **图 3**  高级选项信息<a name="fig1208529493"></a>  
        ![](figures/高级选项信息.png "高级选项信息")


    >![](public_sys-resources/icon-note.gif) **说明：**   
    >在SQL语句所在行的“操作“列，单击“详情“，可以查看SQL语句的详细信息。  

    **表 1**  SQL语句信息参数说明

    <a name="table4295843716304"></a>
    <table><thead align="left"><tr id="row4338993216304"><th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.3.1.1"><p id="p2492361616304"><a name="p2492361616304"></a><a name="p2492361616304"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.39%" id="mcps1.2.3.1.2"><p id="p554697916304"><a name="p554697916304"></a><a name="p554697916304"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row8736194992614"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p27371849182610"><a name="p27371849182610"></a><a name="p27371849182610"></a>序号</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p673724912620"><a name="p673724912620"></a><a name="p673724912620"></a>SQL语句的编号。</p>
    </td>
    </tr>
    <tr id="row3896937416304"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p240275716304"><a name="p240275716304"></a><a name="p240275716304"></a>SQL语句</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p6040559116304"><a name="p6040559116304"></a><a name="p6040559116304"></a>SQL语句的名称。</p>
    </td>
    </tr>
    <tr id="row38169719100"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p11817178103"><a name="p11817178103"></a><a name="p11817178103"></a>客户端IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p781717151012"><a name="p781717151012"></a><a name="p781717151012"></a>客户端的IP地址。</p>
    </td>
    </tr>
    <tr id="row121453182104"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p8145151818109"><a name="p8145151818109"></a><a name="p8145151818109"></a>数据库IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p21451918111019"><a name="p21451918111019"></a><a name="p21451918111019"></a>数据库的IP地址。</p>
    </td>
    </tr>
    <tr id="row1675442617106"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p875482618104"><a name="p875482618104"></a><a name="p875482618104"></a>数据库用户</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p12754192617103"><a name="p12754192617103"></a><a name="p12754192617103"></a>数据库的用户。</p>
    </td>
    </tr>
    <tr id="row1332204111319"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p33321041237"><a name="p33321041237"></a><a name="p33321041237"></a>风险等级</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p189761521111719"><a name="p189761521111719"></a><a name="p189761521111719"></a>SQL语句的风险等级。</p>
    </td>
    </tr>
    <tr id="row0860165713317"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p12331342414"><a name="p12331342414"></a><a name="p12331342414"></a>规则</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p17861057634"><a name="p17861057634"></a><a name="p17861057634"></a>SQL语句的审计规则。</p>
    </td>
    </tr>
    <tr id="row1319658616304"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p6229055916304"><a name="p6229055916304"></a><a name="p6229055916304"></a>操作类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p1237050416304"><a name="p1237050416304"></a><a name="p1237050416304"></a>SQL语句操作的类型。</p>
    </td>
    </tr>
    <tr id="row091816547102"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p1918135431014"><a name="p1918135431014"></a><a name="p1918135431014"></a>生成时间</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p10918155441015"><a name="p10918155441015"></a><a name="p10918155441015"></a>SQL语句生成的时间。</p>
    </td>
    </tr>
    </tbody>
    </table>


