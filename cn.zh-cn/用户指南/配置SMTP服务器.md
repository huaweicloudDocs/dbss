# 配置SMTP服务器<a name="ZH-CN_TOPIC_0111166451"></a>

SMTP服务器用于发送告警邮件。要发送告警，必须配置SMTP服务器。

## 背景信息<a name="zh-cn_topic_0180960089_s07b3bbf1039e4397a526d981de52a312"></a>

用户可以创建多个SMTP服务器，并配置主备SMTP服务器，当主SMTP服务器无法访问时，系统会自动切换到备SMTP服务器来发送告警邮件。配置主备SMTP服务器，请参见[设置系统配置](设置系统配置.md#ZH-CN_TOPIC_0111166461)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>配置SMTP服务器时，默认采用SSL连接。  

## 操作步骤<a name="zh-cn_topic_0180960089_s109d18ea548540b28e2668df2cabf3e5"></a>

1.  在HexaTier主菜单上，单击“系统“。
2.  在导航树上，选择“告警 \> SMTP服务器“。
3.  根据需要执行下列操作：
    -   创建新的SMTP服务器

        在命令栏上，单击“新建“。

    -   编辑已有的SMTP服务器

        找到要编辑的SMTP服务器，然后单击该行末尾的![](figures/编辑-21.png)（编辑）。

4.  配置SMTP服务器详细信息和告警邮件的发件信息，如下表：

    **表 1**  SMTP服务器参数

    <a name="zh-cn_topic_0180960089_tdf4057ce01cb480c9cff75fdd6331140"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180960089_rc5717c46f15f4bf3817d176e63006a02"><th class="cellrowborder" valign="top" width="29.7%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960089_acc221fc66bb94f7cbcfad6135d69cd9e"><a name="zh-cn_topic_0180960089_acc221fc66bb94f7cbcfad6135d69cd9e"></a><a name="zh-cn_topic_0180960089_acc221fc66bb94f7cbcfad6135d69cd9e"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="70.3%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960089_adc7cbb69c5e84acbbd4dd944173bc040"><a name="zh-cn_topic_0180960089_adc7cbb69c5e84acbbd4dd944173bc040"></a><a name="zh-cn_topic_0180960089_adc7cbb69c5e84acbbd4dd944173bc040"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180960089_rbe4f1dc77c164ed3bb2b3dada4563e48"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p596723711067"><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p596723711067"></a><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p596723711067"></a>SMTP服务器名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p16238441067"><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p16238441067"></a><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p16238441067"></a>SMTP服务器的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960089_reacf1f4a289841e583f9bfece8db355b"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_a1f36f112798b46c0b5fc31f5d15d0484"><a name="zh-cn_topic_0180960089_a1f36f112798b46c0b5fc31f5d15d0484"></a><a name="zh-cn_topic_0180960089_a1f36f112798b46c0b5fc31f5d15d0484"></a>SMTP服务器地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_a9625e9e1dde542b48fdd63127a78303b"><a name="zh-cn_topic_0180960089_a9625e9e1dde542b48fdd63127a78303b"></a><a name="zh-cn_topic_0180960089_a9625e9e1dde542b48fdd63127a78303b"></a>SMTP服务器的IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960089_r90ad0263db114b7ea435d16fb4bb959a"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_a7a7d5eb14599456a80acf16c7e17366f"><a name="zh-cn_topic_0180960089_a7a7d5eb14599456a80acf16c7e17366f"></a><a name="zh-cn_topic_0180960089_a7a7d5eb14599456a80acf16c7e17366f"></a>SMTP服务器端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p993647415470"><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p993647415470"></a><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p993647415470"></a>SMTP服务器的传出TCP/IP端口。端口缺省值为<span class="parmvalue" id="zh-cn_topic_0180960089_pa50f828eee8e42e9b2f1244e31873123"><a name="zh-cn_topic_0180960089_pa50f828eee8e42e9b2f1244e31873123"></a><a name="zh-cn_topic_0180960089_pa50f828eee8e42e9b2f1244e31873123"></a>“25”</span>，用户可以根据情况对其进行修改。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960089_rdeabed29d5d14e1383abc9918c780251"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_abd309d26f7db45f2a81be46759e1720a"><a name="zh-cn_topic_0180960089_abd309d26f7db45f2a81be46759e1720a"></a><a name="zh-cn_topic_0180960089_abd309d26f7db45f2a81be46759e1720a"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p281943015473"><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p281943015473"></a><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p281943015473"></a>连接SMTP服务器的用户名。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960089_re7d732ec905d4fab81969f2309d3f78d"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_a3ce9e1dba7674082a173be10f77c95b2"><a name="zh-cn_topic_0180960089_a3ce9e1dba7674082a173be10f77c95b2"></a><a name="zh-cn_topic_0180960089_a3ce9e1dba7674082a173be10f77c95b2"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_adcd6ca8913dc4190922eaf9b38ae0093"><a name="zh-cn_topic_0180960089_adcd6ca8913dc4190922eaf9b38ae0093"></a><a name="zh-cn_topic_0180960089_adcd6ca8913dc4190922eaf9b38ae0093"></a>连接SMTP服务器的密码。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960089_r9e8ca844a54949229112e62e9e56f416"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_a7f7ae7a6156844a9baeec5d75e4617a7"><a name="zh-cn_topic_0180960089_a7f7ae7a6156844a9baeec5d75e4617a7"></a><a name="zh-cn_topic_0180960089_a7f7ae7a6156844a9baeec5d75e4617a7"></a>发出邮箱</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p852591915484"><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p852591915484"></a><a name="zh-cn_topic_0180960089_zh-cn_topic_0076429778_p852591915484"></a>发送告警的电子邮箱。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960089_r063566c46e04437f9513ff7daf3f5dd4"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_a4a80abd9e7cd4cca9b7b53d927a67d70"><a name="zh-cn_topic_0180960089_a4a80abd9e7cd4cca9b7b53d927a67d70"></a><a name="zh-cn_topic_0180960089_a4a80abd9e7cd4cca9b7b53d927a67d70"></a>发出名</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_a8cc0bf10dd2a4094a544b9e0eabf2a98"><a name="zh-cn_topic_0180960089_a8cc0bf10dd2a4094a544b9e0eabf2a98"></a><a name="zh-cn_topic_0180960089_a8cc0bf10dd2a4094a544b9e0eabf2a98"></a>告警发送者的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960089_row954791505110"><td class="cellrowborder" valign="top" width="29.7%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960089_p16547141515113"><a name="zh-cn_topic_0180960089_p16547141515113"></a><a name="zh-cn_topic_0180960089_p16547141515113"></a>收件人邮箱地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.3%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960089_p654771519516"><a name="zh-cn_topic_0180960089_p654771519516"></a><a name="zh-cn_topic_0180960089_p654771519516"></a>接收告警的电子邮箱。</p>
    </td>
    </tr>
    </tbody>
    </table>

5.  单击“测试服务器“。

    验证SMTP服务器设置。

6.  单击“创建“或“更新“。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >请确保在“系统 \> 配置 \> 系统配置“下，“对象关联“设置为“已启用“。  


