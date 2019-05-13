# 查看SQL注入检测信息<a name="ZH-CN_TOPIC_0146120446"></a>

本章节介绍如何查看数据库安全审计的SQL注入检测信息。

## 前提条件<a name="section070891116319"></a>

-   已获取管理控制台的登录账号与密码。
-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   已开启数据库审计，并在数据库端或应用端成功安装Agent。
-   已成功设置审计规则。

## 操作步骤<a name="section20994171263912"></a>

1.  登录管理控制台。
2.  单击管理控制台左上角的![](figures/项目-0.png)，选择区域或项目。
3.  单击管理控制台上方的“服务列表“，选择“安全  \>  数据库安全服务 DBSS“，进入数据库安全防护实例列表界面。
4.  在左侧导航树中，选择“数据库安全服务  \>  数据库安全审计“，进入数据库安全审计实例列表界面。
5.  在数据库安全审计实例列表中，单击需要查看SQL注入检测信息的实例名称，如[图1](#fig7878158164919)所示。

    **图 1**  数据库安全审计实例列表<a name="fig7878158164919"></a>  
    ![](figures/数据库安全审计实例列表.png "数据库安全审计实例列表")

6.  在“实例详情“界面，选择“规则  \>  SQL注入“，进入SQL注入检测列表页面。
7.  查看SQL注入检测信息，如[图2](#fig71914515113)所示，相关参数如[表1](#table964761214306)所示。

    **图 2**  查看SQL注入检测信息<a name="fig71914515113"></a>  
    ![](figures/查看SQL注入检测信息.png "查看SQL注入检测信息")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   选择SQL注入检测的风险级别，列表将显示该级别的SQL注入检测信息。  
    >-   输入SQL注入检测的关键字，单击![](figures/搜索-18.png)或按“Enter“，可以搜索指定的SQL注入检测信息。  

    **表 1**  SQL注入检测信息参数说明

    <a name="table964761214306"></a>
    <table><thead align="left"><tr id="row1365581213011"><th class="cellrowborder" valign="top" width="25.629999999999995%" id="mcps1.2.3.1.1"><p id="p96584127304"><a name="p96584127304"></a><a name="p96584127304"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.37%" id="mcps1.2.3.1.2"><p id="p18660171293013"><a name="p18660171293013"></a><a name="p18660171293013"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1528102263112"><td class="cellrowborder" valign="top" width="25.629999999999995%" headers="mcps1.2.3.1.1 "><p id="p12816221319"><a name="p12816221319"></a><a name="p12816221319"></a>序号</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.37%" headers="mcps1.2.3.1.2 "><p id="p122820222316"><a name="p122820222316"></a><a name="p122820222316"></a>SQL注入检测的编号。</p>
    </td>
    </tr>
    <tr id="row7664312163018"><td class="cellrowborder" valign="top" width="25.629999999999995%" headers="mcps1.2.3.1.1 "><p id="p56657123309"><a name="p56657123309"></a><a name="p56657123309"></a>名称</p>
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


