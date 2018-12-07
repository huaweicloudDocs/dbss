# 登录HexaTier<a name="ZH-CN_TOPIC_0111166411"></a>

用户需要登录HexaTier对开启的DBSS实例进行配置，本章节介绍登录HexaTier的操作。

## 操作场景<a name="section25719543151056"></a>

用户需要登录HexaTier对开启的实例进行配置管理，实现对数据库的安全防护。

-   如果DBSS实例绑定了弹性IP，可以在数据库安全服务界面通过互联网登录到HexaTier或使用DBSS实例同一虚拟私有云中的弹性云服务器登录HexaTier。
-   如果DBSS实例未绑定弹性IP，只能使用DBSS实例同一虚拟私有云中的弹性云服务器登录HexaTier。

## 前提条件<a name="section26173815151056"></a>

-   已获取管理控制台的登录帐号与密码。
-   如果需要在数据库安全服务界面通过互联网登录，DBSS实例必须绑定了弹性IP，且实例的“状态“为“运行中“。
-   已获取登录HexaTier的密码。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >首次登录HexaTier，登录用户名为**admin**，默认密码为购买DBSS实例时设置的HexaTier的登录密码。为了确保用户密码安全性，用户应该定期修改用户密码。密码默认有效期90天，系统会在到期前7天提醒用户修改密码。  

    HexaTier的浏览器满足[表1](#table31027251162210)要求。 

    **表 1**  支持的浏览器版本

    <a name="table31027251162210"></a>
    <table><thead align="left"><tr id="row19104616335"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1010126143316"><a name="p1010126143316"></a><a name="p1010126143316"></a>浏览器</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p12108653312"><a name="p12108653312"></a><a name="p12108653312"></a>版本</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row310565337"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p121086183313"><a name="p121086183313"></a><a name="p121086183313"></a>Google Chrome</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p61012673318"><a name="p61012673318"></a><a name="p61012673318"></a>-</p>
    </td>
    </tr>
    <tr id="row1910156193316"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p14101868333"><a name="p14101868333"></a><a name="p14101868333"></a>Mozilla FireFox</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1710116103311"><a name="p1710116103311"></a><a name="p1710116103311"></a>30.1及以上</p>
    </td>
    </tr>
    <tr id="row181018663319"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p51066113319"><a name="p51066113319"></a><a name="p51066113319"></a>Internet Explorer</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p61110612331"><a name="p61110612331"></a><a name="p61110612331"></a>11.0及以上</p>
    </td>
    </tr>
    </tbody>
    </table>


## 在数据库安全服务界面通过互联网登录<a name="section59621770151056"></a>

1.  登录管理控制台。
2.  单击页面上方的“服务列表“，选择“安全“  \>  “数据库安全服务 DBSS“，进入数据库安全服务界面。
3.  在需要登录HexaTier的实例页面框中，单击“登录“，如[图1](#fig025582318449)所示，系统跳转到该实例的HexaTier登录界面。

    **图 1**  登录HexaTier<a name="fig025582318449"></a>  
    ![](figures/登录HexaTier.png "登录HexaTier")

4.  输入HexaTier的登录用户名**admin**和密码，单击“登录“或按“Enter“，进入HexaTier。

    ![](figures/HexaTier登录页面.png)


## 使用同一虚拟私有云中的弹性云服务器登录<a name="section4560884124237"></a>

1.  在待登录的DBSS实例的同一个虚拟私有云下，查看虚拟私有云中是否存在弹性云服务器。
    -   是：执行[2](#l7ab55acbe3894374a66e9e390f362f36)。
    -   否：在该虚拟机私有云下创建弹性云服务器后，执行[2](#l7ab55acbe3894374a66e9e390f362f36)。

2.  <a name="l7ab55acbe3894374a66e9e390f362f36"></a>使用满足[表2](#t505be23c06ee4bbabed5ab52f8a9539a)要求的浏览器，输入以下地址后。按“Enter“，进入HexaTier的登录界面。
    https://_弹性云服务器的私有IP_:5000
    >![](public_sys-resources/icon-notice.gif) **注意：**   
    >如果不能访问“5000“端口，则需要在安全组中添加TCP（Transmission Control Protocol）的“5000“端口访问权限。详细操作，请参见《虚拟私有云用户指南》。  

    **表 2**  支持的浏览器版本

    <a name="t505be23c06ee4bbabed5ab52f8a9539a"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0111166411_row19104616335"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0111166411_p1010126143316"><a name="zh-cn_topic_0111166411_p1010126143316"></a><a name="zh-cn_topic_0111166411_p1010126143316"></a>浏览器</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0111166411_p12108653312"><a name="zh-cn_topic_0111166411_p12108653312"></a><a name="zh-cn_topic_0111166411_p12108653312"></a>版本</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0111166411_row310565337"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0111166411_p121086183313"><a name="zh-cn_topic_0111166411_p121086183313"></a><a name="zh-cn_topic_0111166411_p121086183313"></a>Google Chrome</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0111166411_p61012673318"><a name="zh-cn_topic_0111166411_p61012673318"></a><a name="zh-cn_topic_0111166411_p61012673318"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0111166411_row1910156193316"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0111166411_p14101868333"><a name="zh-cn_topic_0111166411_p14101868333"></a><a name="zh-cn_topic_0111166411_p14101868333"></a>Mozilla FireFox</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0111166411_p1710116103311"><a name="zh-cn_topic_0111166411_p1710116103311"></a><a name="zh-cn_topic_0111166411_p1710116103311"></a>30.1及以上</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0111166411_row181018663319"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0111166411_p51066113319"><a name="zh-cn_topic_0111166411_p51066113319"></a><a name="zh-cn_topic_0111166411_p51066113319"></a>Internet Explorer</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0111166411_p61110612331"><a name="zh-cn_topic_0111166411_p61110612331"></a><a name="zh-cn_topic_0111166411_p61110612331"></a>11.0及以上</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  输入HexaTier的登录用户名**admin**和密码，单击“登录“或按“Enter“，进入HexaTier。

    ![](figures/HexaTier登录页面.png)


