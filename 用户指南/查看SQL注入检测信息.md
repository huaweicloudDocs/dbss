# 查看SQL注入检测信息<a name="dbss_01_0207"></a>

本章节介绍如何查看数据库安全审计的SQL注入检测信息。

## 前提条件<a name="section070891116319"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   已成功开启数据库安全审计功能。

## 操作步骤<a name="section20994171263912"></a>

1.  [登录管理控制台](https://console.huaweicloud.com/?locale=zh-cn)。
2.  在页面上方选择“区域“后，单击页面左上方的![](figures/icon-list-1.png)，选择“安全与合规  \>  数据库安全服务“，进入数据库安全审计“总览“界面。
3.  在左侧导航树中，选择“审计规则“。
4.  在“选择实例“下拉列表框中，选择需要查看SQL注入检测信息的实例。选择“SQL注入“页签。
5.  查看SQL注入检测信息，如[图1](#fig71914515113)所示，相关参数如[表1](#table964761214306)所示。

    **图 1**  查看SQL注入检测信息<a name="fig71914515113"></a>  
    ![](figures/查看SQL注入检测信息.png "查看SQL注入检测信息")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >在列表右上方“全部风险等级“下拉列表框中选择SQL注入的风险等级，或输入SQL注入名称的关键字，可以搜索指定的SQL注入检测规则。

    **表 1**  SQL注入检测信息参数说明

    <a name="table964761214306"></a>
    <table><thead align="left"><tr id="row1365581213011"><th class="cellrowborder" valign="top" width="25.629999999999995%" id="mcps1.2.3.1.1"><p id="p96584127304"><a name="p96584127304"></a><a name="p96584127304"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.37%" id="mcps1.2.3.1.2"><p id="p18660171293013"><a name="p18660171293013"></a><a name="p18660171293013"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7664312163018"><td class="cellrowborder" valign="top" width="25.629999999999995%" headers="mcps1.2.3.1.1 "><p id="p56657123309"><a name="p56657123309"></a><a name="p56657123309"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.37%" headers="mcps1.2.3.1.2 "><p id="p14669161217308"><a name="p14669161217308"></a><a name="p14669161217308"></a>SQL注入检测的名称。</p>
    </td>
    </tr>
    <tr id="row18114121410321"><td class="cellrowborder" valign="top" width="25.629999999999995%" headers="mcps1.2.3.1.1 "><p id="p195041220123213"><a name="p195041220123213"></a><a name="p195041220123213"></a>SQL命令特征</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.37%" headers="mcps1.2.3.1.2 "><p id="p5506192011323"><a name="p5506192011323"></a><a name="p5506192011323"></a>SQL注入检测的命令特征。</p>
    </td>
    </tr>
    <tr id="row17352133015322"><td class="cellrowborder" valign="top" width="25.629999999999995%" headers="mcps1.2.3.1.1 "><p id="p7313193714329"><a name="p7313193714329"></a><a name="p7313193714329"></a>风险等级</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.37%" headers="mcps1.2.3.1.2 "><p id="p631613374329"><a name="p631613374329"></a><a name="p631613374329"></a>SQL注入检测的风险等级，包括：</p>
    <a name="ul10411345155412"></a><a name="ul10411345155412"></a><ul id="ul10411345155412"><li>高</li><li>中</li><li>低</li><li>无风险</li></ul>
    </td>
    </tr>
    <tr id="row19685121213016"><td class="cellrowborder" valign="top" width="25.629999999999995%" headers="mcps1.2.3.1.1 "><p id="p968710125308"><a name="p968710125308"></a><a name="p968710125308"></a>状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.37%" headers="mcps1.2.3.1.2 "><p id="p186901012163011"><a name="p186901012163011"></a><a name="p186901012163011"></a>SQL注入检测的状态，包括：</p>
    <a name="ul118072149340"></a><a name="ul118072149340"></a><ul id="ul118072149340"><li>已启用</li><li>已禁用</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


