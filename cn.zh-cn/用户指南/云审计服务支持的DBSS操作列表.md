# 云审计服务支持的DBSS操作列表<a name="dbss_01_0142"></a>

数据库安全服务通过云审计服务（Cloud Trace Service，CTS）为用户提供云服务资源的操作记录，记录内容包括用户从管理控制台或者开放API发起的云服务资源操作请求以及每次请求的结果，供用户查询、审计和回溯使用。

云审计服务支持的DBSS操作列表如[表1](#table52008441163754)所示。

**表 1**  云审计服务支持的数据库安全服务操作列表

<a name="table52008441163754"></a>
<table><thead align="left"><tr id="zh-cn_topic_0111166559_row35586605163754"><th class="cellrowborder" valign="top" width="35.55%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0111166559_p63942737163754"><a name="zh-cn_topic_0111166559_p63942737163754"></a><a name="zh-cn_topic_0111166559_p63942737163754"></a>操作名称</p>
</th>
<th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0111166559_p16413837105650"><a name="zh-cn_topic_0111166559_p16413837105650"></a><a name="zh-cn_topic_0111166559_p16413837105650"></a>资源类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.28%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0111166559_p11065000163754"><a name="zh-cn_topic_0111166559_p11065000163754"></a><a name="zh-cn_topic_0111166559_p11065000163754"></a>事件名称</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0111166559_row22991462155616"><td class="cellrowborder" valign="top" width="35.55%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0111166559_p65646959155616"><a name="zh-cn_topic_0111166559_p65646959155616"></a><a name="zh-cn_topic_0111166559_p65646959155616"></a>创建实例</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0111166559_p59026800165451"><a name="zh-cn_topic_0111166559_p59026800165451"></a><a name="zh-cn_topic_0111166559_p59026800165451"></a>dbss</p>
</td>
<td class="cellrowborder" valign="top" width="41.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0111166559_p27686863155616"><a name="zh-cn_topic_0111166559_p27686863155616"></a><a name="zh-cn_topic_0111166559_p27686863155616"></a>createInstance</p>
</td>
</tr>
<tr id="zh-cn_topic_0111166559_row61812375155616"><td class="cellrowborder" valign="top" width="35.55%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0111166559_p52180953155616"><a name="zh-cn_topic_0111166559_p52180953155616"></a><a name="zh-cn_topic_0111166559_p52180953155616"></a>删除实例</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0111166559_p4786566165455"><a name="zh-cn_topic_0111166559_p4786566165455"></a><a name="zh-cn_topic_0111166559_p4786566165455"></a>dbss</p>
</td>
<td class="cellrowborder" valign="top" width="41.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0111166559_p1643209155616"><a name="zh-cn_topic_0111166559_p1643209155616"></a><a name="zh-cn_topic_0111166559_p1643209155616"></a>deleteInstance</p>
</td>
</tr>
<tr id="zh-cn_topic_0111166559_row38095708155616"><td class="cellrowborder" valign="top" width="35.55%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0111166559_p51158909155616"><a name="zh-cn_topic_0111166559_p51158909155616"></a><a name="zh-cn_topic_0111166559_p51158909155616"></a>开启实例</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0111166559_p12500923155616"><a name="zh-cn_topic_0111166559_p12500923155616"></a><a name="zh-cn_topic_0111166559_p12500923155616"></a>dbss</p>
</td>
<td class="cellrowborder" valign="top" width="41.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0111166559_p9980484155616"><a name="zh-cn_topic_0111166559_p9980484155616"></a><a name="zh-cn_topic_0111166559_p9980484155616"></a>startInstance</p>
</td>
</tr>
<tr id="zh-cn_topic_0111166559_row36966343155616"><td class="cellrowborder" valign="top" width="35.55%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0111166559_p20363548155616"><a name="zh-cn_topic_0111166559_p20363548155616"></a><a name="zh-cn_topic_0111166559_p20363548155616"></a>关闭实例</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0111166559_p54846190155616"><a name="zh-cn_topic_0111166559_p54846190155616"></a><a name="zh-cn_topic_0111166559_p54846190155616"></a>dbss</p>
</td>
<td class="cellrowborder" valign="top" width="41.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0111166559_p27978950155616"><a name="zh-cn_topic_0111166559_p27978950155616"></a><a name="zh-cn_topic_0111166559_p27978950155616"></a>stopInstance</p>
</td>
</tr>
<tr id="zh-cn_topic_0111166559_row62477845155616"><td class="cellrowborder" valign="top" width="35.55%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0111166559_p5733644155616"><a name="zh-cn_topic_0111166559_p5733644155616"></a><a name="zh-cn_topic_0111166559_p5733644155616"></a>重启实例</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0111166559_p45509463155616"><a name="zh-cn_topic_0111166559_p45509463155616"></a><a name="zh-cn_topic_0111166559_p45509463155616"></a>dbss</p>
</td>
<td class="cellrowborder" valign="top" width="41.28%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0111166559_p4123095155616"><a name="zh-cn_topic_0111166559_p4123095155616"></a><a name="zh-cn_topic_0111166559_p4123095155616"></a>rebootInstance</p>
</td>
</tr>
</tbody>
</table>

