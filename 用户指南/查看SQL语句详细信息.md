# 查看SQL语句详细信息<a name="dbss_01_0205"></a>

添加的数据库连接到数据库安全审计实例后，您可以查看该数据库详细的SQL语句信息。

## 前提条件<a name="section441811405410"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   已成功开启数据库安全审计功能。

-   数据库安全审计实例已成功添加安全组规则。

## 操作步骤<a name="section16337113512514"></a>

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  在页面上方选择“区域“后，单击页面左上方的![](figures/icon-list-1.png)，选择“安全与合规  \>  数据库安全服务“，进入数据库安全审计“总览“界面。
3.  在“选择实例“下拉列表框中，选择需要查看SQL语句信息的实例。
4.  选择“语句“页签。
5.  查询SQL语句信息，如[图1](#fig78811126122218)所示。

    **图 1**  查询SQL语句<a name="fig78811126122218"></a>  
    ![](figures/查询SQL语句.png "查询SQL语句")

    您可以按照以下方法，查询指定的SQL语句。

    -   选择“时间“（“全部“、“近30分钟“、“近1小时“、“近24小时“、“近7天“或“近30天“），或者单击![](figures/icon-calendar-2.png)，选择开始时间和结束时间，单击“提交“，列表显示该时间段的SQL语句。
    -   选择“风险等级“（“全部“、“高“、“中“、“低“或“信任“），单击“提交“，列表显示该级别的SQL语句。
    -   单击“高级选项“后的![](figures/icon-drop.png)，输入相关信息，如[图2](#fig588352620222)所示，单击“提交“，列表显示该选项的SQL语句。

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >一次查询最多可查询10,000条记录。

        **图 2**  高级选项信息<a name="fig588352620222"></a>  
        ![](figures/高级选项信息.png "高级选项信息")

6.  在需要查看详情的SQL语句所在行的“操作“列，单击“详情“，如[图3](#fig999564692815)所示。

    **图 3**  查看SQL语句详情<a name="fig999564692815"></a>  
    ![](figures/查看SQL语句详情.png "查看SQL语句详情")

7.  在“详情“提示框中，查看SQL语句的详细信息，如[图4](#fig138071753181812)所示，相关参数说明如[表1](#table14884152602217)所示。

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >审计语句和结果集的长度限制为10,240字节。超出部分，系统将不记录在审计日志中。

    **图 4** “详情“提示框<a name="fig138071753181812"></a>  
    ![](figures/详情提示框.png "详情提示框")

    **表 1**  SQL语句详情参数说明

    <a name="table14884152602217"></a>
    <table><thead align="left"><tr id="row118840263228"><th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.3.1.1"><p id="p18842263228"><a name="p18842263228"></a><a name="p18842263228"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.39%" id="mcps1.2.3.1.2"><p id="p128841826182218"><a name="p128841826182218"></a><a name="p128841826182218"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row0884182672210"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p9884202611223"><a name="p9884202611223"></a><a name="p9884202611223"></a>会话ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p9884426142215"><a name="p9884426142215"></a><a name="p9884426142215"></a>SQL语句的ID，由系统自动生成。</p>
    </td>
    </tr>
    <tr id="row96754582306"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p136774585302"><a name="p136774585302"></a><a name="p136774585302"></a>数据库实例</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p067713584301"><a name="p067713584301"></a><a name="p067713584301"></a>SQL语句所在的数据库实例。</p>
    </td>
    </tr>
    <tr id="row59360241310"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p13937112443115"><a name="p13937112443115"></a><a name="p13937112443115"></a>数据库类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p99371224103112"><a name="p99371224103112"></a><a name="p99371224103112"></a>执行SQL语句所在的数据库的类型。</p>
    </td>
    </tr>
    <tr id="row21351542319"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p1513505493120"><a name="p1513505493120"></a><a name="p1513505493120"></a>数据库用户</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p41351154153111"><a name="p41351154153111"></a><a name="p41351154153111"></a>执行SQL语句的数据库用户。</p>
    </td>
    </tr>
    <tr id="row1026112617449"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p9381183113444"><a name="p9381183113444"></a><a name="p9381183113444"></a>客户端MAC地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p202625265445"><a name="p202625265445"></a><a name="p202625265445"></a>执行SQL语句所在客户端MAC地址。</p>
    </td>
    </tr>
    <tr id="row20490164511449"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p11490545184410"><a name="p11490545184410"></a><a name="p11490545184410"></a>数据库MAC地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p1349064510446"><a name="p1349064510446"></a><a name="p1349064510446"></a>执行SQL语句所在数据库MAC地址。</p>
    </td>
    </tr>
    <tr id="row16434161344511"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p20715121419457"><a name="p20715121419457"></a><a name="p20715121419457"></a>客户端IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p187151145457"><a name="p187151145457"></a><a name="p187151145457"></a>执行SQL语句所在客户端的IP地址。</p>
    </td>
    </tr>
    <tr id="row877152318326"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p777152343211"><a name="p777152343211"></a><a name="p777152343211"></a>数据库IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p1777142393212"><a name="p1777142393212"></a><a name="p1777142393212"></a>执行SQL语句所在的数据库的IP地址。</p>
    </td>
    </tr>
    <tr id="row58101733173213"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p12810123315325"><a name="p12810123315325"></a><a name="p12810123315325"></a>客户端端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p10843203013367"><a name="p10843203013367"></a><a name="p10843203013367"></a>执行SQL语句所在的客户端的端口。</p>
    </td>
    </tr>
    <tr id="row8884172642219"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p18294192714516"><a name="p18294192714516"></a><a name="p18294192714516"></a>数据库端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p329410278457"><a name="p329410278457"></a><a name="p329410278457"></a>执行SQL语句所在的数据库的端口。</p>
    </td>
    </tr>
    <tr id="row1285510419334"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p48551946338"><a name="p48551946338"></a><a name="p48551946338"></a>客户端名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p1455164619366"><a name="p1455164619366"></a><a name="p1455164619366"></a>执行SQL语句所在客户端名称。</p>
    </td>
    </tr>
    <tr id="row16682142517336"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p166831425183317"><a name="p166831425183317"></a><a name="p166831425183317"></a>操作类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p20683192520337"><a name="p20683192520337"></a><a name="p20683192520337"></a>SQL语句的操作类型。</p>
    </td>
    </tr>
    <tr id="row107280370331"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p1728133714333"><a name="p1728133714333"></a><a name="p1728133714333"></a>操作对象类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p16549315103716"><a name="p16549315103716"></a><a name="p16549315103716"></a>SQL语句的操作对象的类型。</p>
    </td>
    </tr>
    <tr id="row18524553143310"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p252445316331"><a name="p252445316331"></a><a name="p252445316331"></a>响应结果</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p452435316333"><a name="p452435316333"></a><a name="p452435316333"></a>执行SQL语句的响应结果。</p>
    </td>
    </tr>
    <tr id="row183011125343"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p9830191283420"><a name="p9830191283420"></a><a name="p9830191283420"></a>影响行数</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p201050320389"><a name="p201050320389"></a><a name="p201050320389"></a>执行SQL语句的影响行数。</p>
    </td>
    </tr>
    <tr id="row1292602815344"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p8926172813413"><a name="p8926172813413"></a><a name="p8926172813413"></a>开始时间</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p1292672811348"><a name="p1292672811348"></a><a name="p1292672811348"></a>SQL语句开始执行的时间。</p>
    </td>
    </tr>
    <tr id="row19482153613412"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p048273613343"><a name="p048273613343"></a><a name="p048273613343"></a>应结束时间</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p13482113614348"><a name="p13482113614348"></a><a name="p13482113614348"></a>SQL语句结束的时间。</p>
    </td>
    </tr>
    <tr id="row1199125143518"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p19991354357"><a name="p19991354357"></a><a name="p19991354357"></a>SQL请求语句</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p89910510352"><a name="p89910510352"></a><a name="p89910510352"></a>SQL语句的名称。</p>
    </td>
    </tr>
    <tr id="row96020195358"><td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.3.1.1 "><p id="p5601519163512"><a name="p5601519163512"></a><a name="p5601519163512"></a>请求结果</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.39%" headers="mcps1.2.3.1.2 "><p id="p176091916351"><a name="p176091916351"></a><a name="p176091916351"></a>SQL语句请求执行的结果。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 相关操作<a name="section15790154115115"></a>

-   如果SQL语句列表中未显示输入的SQL语句，说明Agent与数据库安全审计实例之间网络通信异常，请参照[如何处理Agent与数据库安全审计实例之间通信异常？](https://support.huaweicloud.com/dbss_faq/dbss_01_0246.html)处理。

-   数据库开启SSL时，将不能使用数据库安全审计功能。如果您需要使用数据库安全审计功能，请关闭数据库的SSL。关闭数据库SSL的详细操作，请参见[如何关闭数据库SSL？](https://support.huaweicloud.com/dbss_faq/dbss_01_0283.html)。

