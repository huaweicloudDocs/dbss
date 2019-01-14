# HexaTier配置流程<a name="ZH-CN_TOPIC_0111166458"></a>

登录HexaTier后，需要在HexaTier上对DBSS实例进行安全防护配置操作，才可以对接华为云上的数据库，对数据库提供防护和审计功能。

HexaTier的配置流程如[图1](#fig18350802165225)所示，流程说明如[表1](#table443217583618)所示。

**图 1**  HexaTier配置流程<a name="fig18350802165225"></a>  
![](figures/HexaTier配置流程.png "HexaTier配置流程")

**表 1**  HexaTier配置流程说明

<a name="table443217583618"></a>
<table><thead align="left"><tr id="row143210517368"><th class="cellrowborder" valign="top" width="6.360636063606361%" id="mcps1.2.4.1.1"><p id="p243211514369"><a name="p243211514369"></a><a name="p243211514369"></a>序号</p>
</th>
<th class="cellrowborder" valign="top" width="26.162616261626166%" id="mcps1.2.4.1.2"><p id="p10432145183617"><a name="p10432145183617"></a><a name="p10432145183617"></a>配置操作</p>
</th>
<th class="cellrowborder" valign="top" width="67.47674767476747%" id="mcps1.2.4.1.3"><p id="p144326520369"><a name="p144326520369"></a><a name="p144326520369"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1943217515366"><td class="cellrowborder" valign="top" width="6.360636063606361%" headers="mcps1.2.4.1.1 "><p id="p4432175193615"><a name="p4432175193615"></a><a name="p4432175193615"></a>1</p>
</td>
<td class="cellrowborder" valign="top" width="26.162616261626166%" headers="mcps1.2.4.1.2 "><p id="p1543216553611"><a name="p1543216553611"></a><a name="p1543216553611"></a><a href="登录HexaTier.md">登录HexaTier</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.47674767476747%" headers="mcps1.2.4.1.3 "><p id="p16432452361"><a name="p16432452361"></a><a name="p16432452361"></a>登录HexaTier后，对DBSS实例进行配置管理，实现数据库的安全防护。</p>
</td>
</tr>
<tr id="row14423186183810"><td class="cellrowborder" valign="top" width="6.360636063606361%" headers="mcps1.2.4.1.1 "><p id="p144239614388"><a name="p144239614388"></a><a name="p144239614388"></a>2</p>
</td>
<td class="cellrowborder" valign="top" width="26.162616261626166%" headers="mcps1.2.4.1.2 "><p id="p184232615387"><a name="p184232615387"></a><a name="p184232615387"></a><a href="配置HexaTier日志存储位置.md">配置HexaTier日志存储位置</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.47674767476747%" headers="mcps1.2.4.1.3 "><p id="p11423206133810"><a name="p11423206133810"></a><a name="p11423206133810"></a>配置日志存储位置之后，可以启用监控功能和查看日志记录功能。</p>
</td>
</tr>
<tr id="row695902133817"><td class="cellrowborder" valign="top" width="6.360636063606361%" headers="mcps1.2.4.1.1 "><p id="p129601821386"><a name="p129601821386"></a><a name="p129601821386"></a>3</p>
</td>
<td class="cellrowborder" valign="top" width="26.162616261626166%" headers="mcps1.2.4.1.2 "><p id="p109608283813"><a name="p109608283813"></a><a name="p109608283813"></a><a href="配置受保护的数据库.md">配置受保护的数据库</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.47674767476747%" headers="mcps1.2.4.1.3 "><p id="p49601921380"><a name="p49601921380"></a><a name="p49601921380"></a>配置连接受保护的数据库实例后，用户可以通过HexaTier控制台进行相关配置，启用敏感数据发现、防拖库、数据库防火墙、数据库活动监控和动态数据脱敏等功能。</p>
</td>
</tr>
<tr id="row1539171014387"><td class="cellrowborder" rowspan="5" valign="top" width="6.360636063606361%" headers="mcps1.2.4.1.1 "><p id="p12390102381"><a name="p12390102381"></a><a name="p12390102381"></a>4</p>
</td>
<td class="cellrowborder" valign="top" width="26.162616261626166%" headers="mcps1.2.4.1.2 "><p id="p1112145916187"><a name="p1112145916187"></a><a name="p1112145916187"></a><a href="数据库安全策略简介.md">配置数据库安全策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="67.47674767476747%" headers="mcps1.2.4.1.3 "><p id="p16327204981815"><a name="p16327204981815"></a><a name="p16327204981815"></a>数据库安全策略是保护数据库安全的核心机制，当违反数据库安全策略时，用户可以阻断并立即告警。</p>
</td>
</tr>
<tr id="row11501104718186"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p25191013121914"><a name="p25191013121914"></a><a name="p25191013121914"></a><a href="敏感数据发现策略简介.md">配置敏感数据发现策略</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p5501247121814"><a name="p5501247121814"></a><a name="p5501247121814"></a>可以自动识别并分类数据库中的敏感数据。当HexaTier识别到敏感数据时，用户可以选择自动生成脱敏策略和审计策略。</p>
</td>
</tr>
<tr id="row24472431914"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p813510247196"><a name="p813510247196"></a><a name="p813510247196"></a><a href="数据库防拖库策略简介.md">配置数据库防拖库策略</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p4447184191913"><a name="p4447184191913"></a><a name="p4447184191913"></a>可以对未授权用户、IP地址和应用在数据库特定表中的数据操作进行检测，避免数据泄露。</p>
</td>
</tr>
<tr id="row149741016181920"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p2863632171912"><a name="p2863632171912"></a><a name="p2863632171912"></a><a href="数据库活动监控策略简介.md">配置数据库活动监控策略</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p69758163191"><a name="p69758163191"></a><a name="p69758163191"></a>数据库活动监控也称为数据库审计，用户可以根据自己实际情况选择审计范围，HexaTier将根据用户选择的审校范围，提供数据库的所有操作信息。</p>
</td>
</tr>
<tr id="row912122761910"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p5402434181913"><a name="p5402434181913"></a><a name="p5402434181913"></a><a href="动态数据脱敏策略简介.md">配置动态数据脱敏策略</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p17122202711193"><a name="p17122202711193"></a><a name="p17122202711193"></a>HexaTier提供的实时数据脱敏功能，确保数据库用户敏感信息不被泄露。</p>
</td>
</tr>
</tbody>
</table>

