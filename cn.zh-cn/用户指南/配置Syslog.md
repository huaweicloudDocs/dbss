# 配置Syslog<a name="ZH-CN_TOPIC_0111166474"></a>

用户可以通过系统设置，将信息发送到运行Syslog服务器的远程计算机。Syslog标准用于从网络设备捕获日志信息。

## 操作步骤<a name="zh-cn_topic_0180960129_s569dfbfc197640cb861d89d7e71c83b9"></a>

1.  在HexaTier主菜单上，单击“系统“。
2.  在导航树上，选择“日志 \> Syslog设置“。
3.  在Syslog设置工作区中，配置以下参数：

    **表 1**  日志设置参数

    <a name="zh-cn_topic_0180960129_ta5a6ace5264a4ea7a42cb4789f356276"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180960129_r76c562b450ea4bf4a296a4bbf7a580a8"><th class="cellrowborder" valign="top" width="27.439999999999998%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960129_acfc0d5af7a364caba7878573bc5ca2cc"><a name="zh-cn_topic_0180960129_acfc0d5af7a364caba7878573bc5ca2cc"></a><a name="zh-cn_topic_0180960129_acfc0d5af7a364caba7878573bc5ca2cc"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="72.56%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960129_a6b093daeb0df4e8f992dc1efb6d59fc9"><a name="zh-cn_topic_0180960129_a6b093daeb0df4e8f992dc1efb6d59fc9"></a><a name="zh-cn_topic_0180960129_a6b093daeb0df4e8f992dc1efb6d59fc9"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180960129_r42d15cdb93634cbeb26ca9d07b22f199"><td class="cellrowborder" valign="top" width="27.439999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960129_ad78da489509b4f87ac07090a67e584d7"><a name="zh-cn_topic_0180960129_ad78da489509b4f87ac07090a67e584d7"></a><a name="zh-cn_topic_0180960129_ad78da489509b4f87ac07090a67e584d7"></a>状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.56%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960129_a76c22308e63d4967b6ea18b8e7dccd78"><a name="zh-cn_topic_0180960129_a76c22308e63d4967b6ea18b8e7dccd78"></a><a name="zh-cn_topic_0180960129_a76c22308e63d4967b6ea18b8e7dccd78"></a>启用或禁用Syslog服务器写入。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960129_r86ad56f3bc904d4c85c6d680a28d6ec1"><td class="cellrowborder" valign="top" width="27.439999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960129_a28922458f1c24724b30dddb3001d0832"><a name="zh-cn_topic_0180960129_a28922458f1c24724b30dddb3001d0832"></a><a name="zh-cn_topic_0180960129_a28922458f1c24724b30dddb3001d0832"></a>主机/IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.56%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960129_ab453781c17bb484eb54fcd4763891972"><a name="zh-cn_topic_0180960129_ab453781c17bb484eb54fcd4763891972"></a><a name="zh-cn_topic_0180960129_ab453781c17bb484eb54fcd4763891972"></a>远程Syslog服务器的IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960129_zh-cn_topic_0076429697_row2310315817"><td class="cellrowborder" valign="top" width="27.439999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960129_zh-cn_topic_0076429697_p187134415817"><a name="zh-cn_topic_0180960129_zh-cn_topic_0076429697_p187134415817"></a><a name="zh-cn_topic_0180960129_zh-cn_topic_0076429697_p187134415817"></a>Syslog服务器端口（UDP）</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.56%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960129_ae73a492cf5be4b75a9724f4e584aa986"><a name="zh-cn_topic_0180960129_ae73a492cf5be4b75a9724f4e584aa986"></a><a name="zh-cn_topic_0180960129_ae73a492cf5be4b75a9724f4e584aa986"></a>默认情况下，Syslog服务器监听<span class="parmvalue" id="zh-cn_topic_0180960129_pe26cc3b79d654993b125608238d1be87"><a name="zh-cn_topic_0180960129_pe26cc3b79d654993b125608238d1be87"></a><a name="zh-cn_topic_0180960129_pe26cc3b79d654993b125608238d1be87"></a>“514”</span>端口，通过UDP连接执行通信。如果需要，用户可以修改此端口。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960129_r452aa677304c4b39b540cd5d68e40588"><td class="cellrowborder" valign="top" width="27.439999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960129_a27e70bb67219413f853b70b3ebb6faf8"><a name="zh-cn_topic_0180960129_a27e70bb67219413f853b70b3ebb6faf8"></a><a name="zh-cn_topic_0180960129_a27e70bb67219413f853b70b3ebb6faf8"></a>最低严重性</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.56%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960129_a0380e340151e4c46bc00155fa20e97e4"><a name="zh-cn_topic_0180960129_a0380e340151e4c46bc00155fa20e97e4"></a><a name="zh-cn_topic_0180960129_a0380e340151e4c46bc00155fa20e97e4"></a>发送到Syslog服务器的最低严重级别。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960129_rd3bcbfa180854034a97852edc46c7952"><td class="cellrowborder" valign="top" width="27.439999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960129_ad6d73362d61042f3adbb1b7e7579007d"><a name="zh-cn_topic_0180960129_ad6d73362d61042f3adbb1b7e7579007d"></a><a name="zh-cn_topic_0180960129_ad6d73362d61042f3adbb1b7e7579007d"></a>设施</p>
    </td>
    <td class="cellrowborder" valign="top" width="72.56%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960129_a6753cc2f72ec45aca7e10cf757d2415c"><a name="zh-cn_topic_0180960129_a6753cc2f72ec45aca7e10cf757d2415c"></a><a name="zh-cn_topic_0180960129_a6753cc2f72ec45aca7e10cf757d2415c"></a>发送到Syslog服务器的告警类型。</p>
    </td>
    </tr>
    </tbody>
    </table>

4.  单击“测试“向Syslog服务器发送测试消息。
5.  单击“更新“，应用设置。

