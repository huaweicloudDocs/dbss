# 配置LDAP模式<a name="ZH-CN_TOPIC_0111166435"></a>

配置LDAP集成模式表示HexaTier通过LDAP服务器进行身份验证。只有在系统中配置了LDAP集成模式之后才能添加活动目录用户。

## 操作场景<a name="zh-cn_topic_0110574973_s395d32027447478a958606ffe3ebba53"></a>

该任务指导用户配置LDAP集成模式。

>![](public_sys-resources/icon-note.gif) **说明：**   
>LDAP默认采用SSL连接。  

## 前提条件<a name="zh-cn_topic_0110574973_s0edc600c42d7404485e0269121aaf3e1"></a>

必须禁用高可用性模式才能配置LDAP集成模式。

## 操作步骤<a name="zh-cn_topic_0110574973_sa9f4ab4e4bd24470972dae1032ddcf6c"></a>

1.  在HexaTier主菜单上，单击“资源“。
2.  在导航树上，选择“活动目录“。
3.  在“集成模式“下拉框中选择“LDAP“。

    ![](figures/LDAP集成模式.png)

4.  根据需要设置相关参数：

    **表 1**  配置LDAP模式参数

    <a name="zh-cn_topic_0110574973_t73b33c931da3471a8a07838c163e8459"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0110574973_r5c441d2cfdd044feb93080cd7045d1df"><th class="cellrowborder" valign="top" width="20.49%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0110574973_afe108c1a59a841699019c3c75c2ec21e"><a name="zh-cn_topic_0110574973_afe108c1a59a841699019c3c75c2ec21e"></a><a name="zh-cn_topic_0110574973_afe108c1a59a841699019c3c75c2ec21e"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="79.51%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0110574973_aba730a35c1034ecb8dccb52b2b484c19"><a name="zh-cn_topic_0110574973_aba730a35c1034ecb8dccb52b2b484c19"></a><a name="zh-cn_topic_0110574973_aba730a35c1034ecb8dccb52b2b484c19"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0110574973_rae593fa517c948b6bf02daf6b686c088"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574973_zh-cn_topic_0076429813_p529377164625"><a name="zh-cn_topic_0110574973_zh-cn_topic_0076429813_p529377164625"></a><a name="zh-cn_topic_0110574973_zh-cn_topic_0076429813_p529377164625"></a>服务器地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.51%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574973_addb3f1e33ff54ab88cfc784721c4051b"><a name="zh-cn_topic_0110574973_addb3f1e33ff54ab88cfc784721c4051b"></a><a name="zh-cn_topic_0110574973_addb3f1e33ff54ab88cfc784721c4051b"></a>LDAP服务器地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574973_r6b99566863ae4fd1a14c9714a71d7373"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574973_add5eed8ae8f84dc3a9293747e7e37a28"><a name="zh-cn_topic_0110574973_add5eed8ae8f84dc3a9293747e7e37a28"></a><a name="zh-cn_topic_0110574973_add5eed8ae8f84dc3a9293747e7e37a28"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.51%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574973_a1249b24e73c74f9ea986dbddc4571beb"><a name="zh-cn_topic_0110574973_a1249b24e73c74f9ea986dbddc4571beb"></a><a name="zh-cn_topic_0110574973_a1249b24e73c74f9ea986dbddc4571beb"></a>连接LDAP服务器的端口。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574973_r020eec6ea7ac40878a51bbbc09a2f4bd"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574973_a150909ed8b88422e8600aea18fff1592"><a name="zh-cn_topic_0110574973_a150909ed8b88422e8600aea18fff1592"></a><a name="zh-cn_topic_0110574973_a150909ed8b88422e8600aea18fff1592"></a>加密</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.51%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574973_a78f09c353eaf4e67abbe33c7786d68a2"><a name="zh-cn_topic_0110574973_a78f09c353eaf4e67abbe33c7786d68a2"></a><a name="zh-cn_topic_0110574973_a78f09c353eaf4e67abbe33c7786d68a2"></a>与LDAP服务器的连接加密方式，包含以下三种：</p>
    <a name="zh-cn_topic_0110574973_u21f4cf3d9cf94774836f63a26c54f309"></a><a name="zh-cn_topic_0110574973_u21f4cf3d9cf94774836f63a26c54f309"></a><ul id="zh-cn_topic_0110574973_u21f4cf3d9cf94774836f63a26c54f309"><li>无</li><li>LDAPS：HexaTier通过使用SSL的LDAP进行身份验证。</li><li>STARTTLS：对纯文本通信协议的扩展，将不安全的连接升级为加密连接。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574973_r7ac236c9d6044c0daed9cf7298b55812"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574973_a2bb224e3d3d044449606fa7844460564"><a name="zh-cn_topic_0110574973_a2bb224e3d3d044449606fa7844460564"></a><a name="zh-cn_topic_0110574973_a2bb224e3d3d044449606fa7844460564"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.51%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574973_a788f25340654406f975bf3fe1053c651"><a name="zh-cn_topic_0110574973_a788f25340654406f975bf3fe1053c651"></a><a name="zh-cn_topic_0110574973_a788f25340654406f975bf3fe1053c651"></a>连接LDAP服务器的用户名。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574973_r68402b14500746e79570d3a2482da22f"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574973_a7fde6d111d0440598ec70fb7978461fb"><a name="zh-cn_topic_0110574973_a7fde6d111d0440598ec70fb7978461fb"></a><a name="zh-cn_topic_0110574973_a7fde6d111d0440598ec70fb7978461fb"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.51%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574973_zh-cn_topic_0076429813_p136351446594"><a name="zh-cn_topic_0110574973_zh-cn_topic_0076429813_p136351446594"></a><a name="zh-cn_topic_0110574973_zh-cn_topic_0076429813_p136351446594"></a>连接LDAP服务器的密码。</p>
    </td>
    </tr>
    </tbody>
    </table>

5.  单击“测试连接“。

    显示状态消息，提示测试连接成功或失败。

6.  测试成功后，单击“更新“。

    更新会自动测试与用户设置的连接。出现状态消息，提示连接成功或失败。


