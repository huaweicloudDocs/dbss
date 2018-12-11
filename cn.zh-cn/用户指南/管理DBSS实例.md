# 管理DBSS实例<a name="ZH-CN_TOPIC_0111166508"></a>

用户成功购买DBSS实例后，可以查看实例信息，重启、开启或关闭实例。

## 前提条件<a name="section97118228499"></a>

-   已获取管理控制台的登录帐号与密码。
-   已成功购买DBSS实例。
-   重启实例和关闭实例前，请确认实例的“运行状态“为“运行中“。
-   开启实例前，请确认实例的“运行状态“为“已关闭“。

## 查看实例信息<a name="section1688216416315"></a>

1.  登录管理控制台。
2.  单击页面上方的“服务列表“，选择“安全  \>  数据库安全服务 DBSS“，进入数据库安全服务界面。
3.  查看DBSS实例的信息，如[图1](#fig1325745611915)所示，相关参数说明如[表1](#table1025994517211)所示。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >在实例列表中，单击实例前面的![](figures/实例详情.png)，可以查看该实例的详细信息。  

    **图 1**  查看实例信息<a name="fig1325745611915"></a>  
    ![](figures/查看实例信息.png "查看实例信息")

    **表 1**  实例信息参数说明

    <a name="table1025994517211"></a>
    <table><thead align="left"><tr id="row1626074517217"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.3.1.1"><p id="p9260045112114"><a name="p9260045112114"></a><a name="p9260045112114"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="83%" id="mcps1.2.3.1.2"><p id="p7260194582118"><a name="p7260194582118"></a><a name="p7260194582118"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18260134511215"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.3.1.1 "><p id="p62601045112117"><a name="p62601045112117"></a><a name="p62601045112117"></a>实例名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="83%" headers="mcps1.2.3.1.2 "><p id="p13698174652218"><a name="p13698174652218"></a><a name="p13698174652218"></a>实例的名称。</p>
    </td>
    </tr>
    <tr id="row326014459212"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.3.1.1 "><p id="p16763165610222"><a name="p16763165610222"></a><a name="p16763165610222"></a>版本</p>
    </td>
    <td class="cellrowborder" valign="top" width="83%" headers="mcps1.2.3.1.2 "><p id="p47630567221"><a name="p47630567221"></a><a name="p47630567221"></a>实例的服务版本。</p>
    </td>
    </tr>
    <tr id="row12260124518212"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.3.1.1 "><p id="p17260845122119"><a name="p17260845122119"></a><a name="p17260845122119"></a>连接地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="83%" headers="mcps1.2.3.1.2 "><p id="p192608458211"><a name="p192608458211"></a><a name="p192608458211"></a>应用连接实例的私有IP地址。</p>
    </td>
    </tr>
    <tr id="row11260124513215"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.3.1.1 "><p id="p1726044518211"><a name="p1726044518211"></a><a name="p1726044518211"></a>运行状态</p>
    </td>
    <td class="cellrowborder" valign="top" width="83%" headers="mcps1.2.3.1.2 "><p id="p1260745162119"><a name="p1260745162119"></a><a name="p1260745162119"></a>实例当前的运行状态，包括：</p>
    <a name="ul108156241253"></a><a name="ul108156241253"></a><ul id="ul108156241253"><li>运行中</li><li>创建中</li><li>故障</li><li>已关闭</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


## 重启实例<a name="section11202812165017"></a>

1.  登录管理控制台。
2.  单击页面上方的“服务列表“，选择“安全  \>  数据库安全服务 DBSS“，进入数据库安全服务界面。
3.  单击需要重启的DBSS实例。
4.  在需要重启的实例所在行，单击“重启“，如[图2](#fig78715132217)所示。

    **图 2**  重启实例<a name="fig78715132217"></a>  
    ![](figures/重启实例.png "重启实例")

5.  在弹出的提示对话框中，单击“确定“，如[图3](#fig97781991740)所示。

    **图 3** “重启“对话框<a name="fig97781991740"></a>  
    ![](figures/重启对话框.png "重启对话框")

    单击实例列表右上方的![](figures/刷新.png)刷新界面，实例重启成功。


## 开启实例<a name="section586111276377"></a>

成功购买DBSS实例后，实例自动开启。开启实例后，用户可以登录HexaTier对实例进行配置管理，实现对数据库的安全防护。

当实例关闭后，如果需要登录HexaTier，则需要开启实例。

1.  登录管理控制台。
2.  单击页面上方的“服务列表“，选择“安全  \>  数据库安全服务 DBSS“，进入数据库安全服务界面。
3.  单击需要开启的DBSS实例。
4.  在需要开启的实例所在行，单击“开启“，如[图4](#fig14477185813019)所示。

    **图 4**  开启实例<a name="fig14477185813019"></a>  
    ![](figures/开启实例.png "开启实例")

5.  在弹出的提示对话框中，单击“确定“。

    开启实例成功，实例的“运行状态“为“运行中“。


## 关闭实例<a name="section464917201380"></a>

关闭实例后，将不能登录HexaTier对实例进行配置管理。

1.  登录管理控制台。
2.  单击页面上方的“服务列表“，选择“安全  \>  数据库安全服务 DBSS“，进入数据库安全服务界面。
3.  单击需要关闭的DBSS实例。
4.  在需要关闭的实例所在行，单击“关闭“，如[图5](#fig17998195641819)所示。

    **图 5**  关闭实例<a name="fig17998195641819"></a>  
    ![](figures/关闭实例.png "关闭实例")

5.  在弹出的提示对话框中，单击“确定“，如[图6](#fig3772102813313)所示。

    **图 6** “关闭“对话框<a name="fig3772102813313"></a>  
    ![](figures/关闭对话框.png "关闭对话框")

    关闭实例成功，实例的“状态“为“已关闭“。


