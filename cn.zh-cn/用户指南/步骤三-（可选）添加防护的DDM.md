# 步骤三：（可选）添加防护的DDM<a name="ZH-CN_TOPIC_0121926605"></a>

DDM即分布式数据库中间件（Distributed Database Middleware，简称DDM），专注于解决数据库分布式扩展问题，突破了传统数据库的容量和性能瓶颈，实现海量数据高并发访问。HexaTier支持以DDM作为受保护的数据库，并提供相应防护功能。

## 背景信息<a name="zh-cn_topic_0180960123_section686515561145"></a>

DDM使用云数据库MySQL作为存储引擎，具备自动部署、分库分表、弹性伸缩、高可用等全生命周期运维管控能力。

## 操作步骤<a name="zh-cn_topic_0180960123_section5582172252"></a>

1.  获取DDM实例信息。
    1.  登录管理控制台。
    2.  在服务列表，选择“数据库 \> 分布式数据库中间件DDM“。
    3.  在导航栏，单击“DDM实例管理“。

        **图 1**  DDM实例管理<a name="zh-cn_topic_0180960123_fig19754184118420"></a>  
        ![](figures/DDM实例管理.png "DDM实例管理")

    4.  <a name="zh-cn_topic_0180960123_li15771276415"></a>单击DDM实例名称，进入实例基本信息界面，获取实例连接地址。如下图所示：

        **图 2**  DDM实例基本信息<a name="zh-cn_topic_0180960123_fig1151515201944"></a>  
        ![](figures/DDM实例基本信息.png "DDM实例基本信息")

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >一个DDM实例可以有多个连接地址，用户需要针对DDM实例的多个连接地址分别配置受保护的数据库。  

    5.  <a name="zh-cn_topic_0180960123_li02933341344"></a>单击“逻辑库管理“页签，获取逻辑库名称。

        **图 3**  DDM实例逻辑库列表<a name="zh-cn_topic_0180960123_fig138795119518"></a>  
        ![](figures/DDM实例逻辑库列表.png "DDM实例逻辑库列表")

    6.  <a name="zh-cn_topic_0180960123_li41698615142"></a>单击“帐号管理“页签，创建拥有所有逻辑库可读权限的DDM帐号，并记录帐号。

        创建DDM帐号，请参见《分布式数据库中间件用户指南》。

2.  配置受保护的数据库。

    1.  登录HexaTier控制台。
    2.  在HexaTier主菜单上，单击“资源“。
    3.  在命令栏，单击“新建“。
    4.  “数据库类型“选择“MySQL“，并配置以下参数信息。

        **表 1**  数据库参数

        <a name="zh-cn_topic_0180960123_table1389095324610"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0180960123_row108902534462"><th class="cellrowborder" valign="top" width="23.68%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960123_p16890853114616"><a name="zh-cn_topic_0180960123_p16890853114616"></a><a name="zh-cn_topic_0180960123_p16890853114616"></a>参数名称</p>
        </th>
        <th class="cellrowborder" valign="top" width="76.32%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960123_p16890253174611"><a name="zh-cn_topic_0180960123_p16890253174611"></a><a name="zh-cn_topic_0180960123_p16890253174611"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0180960123_row689014536469"><td class="cellrowborder" valign="top" width="23.68%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p14890185354617"><a name="zh-cn_topic_0180960123_p14890185354617"></a><a name="zh-cn_topic_0180960123_p14890185354617"></a>数据库服务器地址</p>
        </td>
        <td class="cellrowborder" valign="top" width="76.32%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p7890453104616"><a name="zh-cn_topic_0180960123_p7890453104616"></a><a name="zh-cn_topic_0180960123_p7890453104616"></a><a href="#zh-cn_topic_0180960123_li15771276415">步骤1.d</a>中记录的DDM连接地址中的IP地址。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row12890653184613"><td class="cellrowborder" valign="top" width="23.68%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p189095334615"><a name="zh-cn_topic_0180960123_p189095334615"></a><a name="zh-cn_topic_0180960123_p189095334615"></a>端口</p>
        </td>
        <td class="cellrowborder" valign="top" width="76.32%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p28901553134619"><a name="zh-cn_topic_0180960123_p28901553134619"></a><a name="zh-cn_topic_0180960123_p28901553134619"></a><a href="#zh-cn_topic_0180960123_li15771276415">步骤1.d</a>中记录的DDM连接地址中的端口号。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row8890053124611"><td class="cellrowborder" valign="top" width="23.68%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p178907533465"><a name="zh-cn_topic_0180960123_p178907533465"></a><a name="zh-cn_topic_0180960123_p178907533465"></a>名称</p>
        </td>
        <td class="cellrowborder" valign="top" width="76.32%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p589016532464"><a name="zh-cn_topic_0180960123_p589016532464"></a><a name="zh-cn_topic_0180960123_p589016532464"></a>连接的数据库实例的别名，HexaTier会自动生成名称，用户也可以自定义该名称。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row38901253174614"><td class="cellrowborder" valign="top" width="23.68%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p14890553184610"><a name="zh-cn_topic_0180960123_p14890553184610"></a><a name="zh-cn_topic_0180960123_p14890553184610"></a>默认数据库</p>
        </td>
        <td class="cellrowborder" valign="top" width="76.32%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p4890353114614"><a name="zh-cn_topic_0180960123_p4890353114614"></a><a name="zh-cn_topic_0180960123_p4890353114614"></a><a href="#zh-cn_topic_0180960123_li02933341344">步骤1.e</a>中记录的逻辑库名称。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row48901753104616"><td class="cellrowborder" valign="top" width="23.68%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p8890205316462"><a name="zh-cn_topic_0180960123_p8890205316462"></a><a name="zh-cn_topic_0180960123_p8890205316462"></a>鉴权方式</p>
        </td>
        <td class="cellrowborder" valign="top" width="76.32%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p1989035318461"><a name="zh-cn_topic_0180960123_p1989035318461"></a><a name="zh-cn_topic_0180960123_p1989035318461"></a>默认为SQL鉴权。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row9890205314612"><td class="cellrowborder" valign="top" width="23.68%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p11890165311465"><a name="zh-cn_topic_0180960123_p11890165311465"></a><a name="zh-cn_topic_0180960123_p11890165311465"></a>用户名</p>
        </td>
        <td class="cellrowborder" valign="top" width="76.32%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p15890145384620"><a name="zh-cn_topic_0180960123_p15890145384620"></a><a name="zh-cn_topic_0180960123_p15890145384620"></a><a href="#zh-cn_topic_0180960123_li41698615142">步骤1.f</a>中创建的DDM可读帐号。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row6890115312465"><td class="cellrowborder" valign="top" width="23.68%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p12890653124615"><a name="zh-cn_topic_0180960123_p12890653124615"></a><a name="zh-cn_topic_0180960123_p12890653124615"></a>密码</p>
        </td>
        <td class="cellrowborder" valign="top" width="76.32%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p7890165334613"><a name="zh-cn_topic_0180960123_p7890165334613"></a><a name="zh-cn_topic_0180960123_p7890165334613"></a><a href="#zh-cn_topic_0180960123_li41698615142">步骤1.f</a>中创建的DDM可读帐号密码。</p>
        </td>
        </tr>
        </tbody>
        </table>

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >一个DDM实例可以有多个连接地址，用户需要针对DDM实例的多个连接地址分别配置受保护的数据库。  

    5.  配置高级代理配置。

        **表 2**  高级代理配置参数

        <a name="zh-cn_topic_0180960123_table2090725374618"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0180960123_row19907155320466"><th class="cellrowborder" valign="top" width="24.81%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960123_p199071753144619"><a name="zh-cn_topic_0180960123_p199071753144619"></a><a name="zh-cn_topic_0180960123_p199071753144619"></a>参数名称</p>
        </th>
        <th class="cellrowborder" valign="top" width="75.19%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960123_p790755374610"><a name="zh-cn_topic_0180960123_p790755374610"></a><a name="zh-cn_topic_0180960123_p790755374610"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0180960123_row119071553104612"><td class="cellrowborder" valign="top" width="24.81%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p290775324611"><a name="zh-cn_topic_0180960123_p290775324611"></a><a name="zh-cn_topic_0180960123_p290775324611"></a>代理标签</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.19%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p169071753114613"><a name="zh-cn_topic_0180960123_p169071753114613"></a><a name="zh-cn_topic_0180960123_p169071753114613"></a>代理的逻辑名称。用户可以自定义该名称。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row189071053104613"><td class="cellrowborder" valign="top" width="24.81%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p2907165310461"><a name="zh-cn_topic_0180960123_p2907165310461"></a><a name="zh-cn_topic_0180960123_p2907165310461"></a>监听地址</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.19%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p59078534465"><a name="zh-cn_topic_0180960123_p59078534465"></a><a name="zh-cn_topic_0180960123_p59078534465"></a>指定用户想要代理监听的IP地址。</p>
        <p id="zh-cn_topic_0180960123_p09071553104611"><a name="zh-cn_topic_0180960123_p09071553104611"></a><a name="zh-cn_topic_0180960123_p09071553104611"></a>用户可以使用0.0.0.0来监听所有IP。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row13907753134614"><td class="cellrowborder" valign="top" width="24.81%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p49077530469"><a name="zh-cn_topic_0180960123_p49077530469"></a><a name="zh-cn_topic_0180960123_p49077530469"></a>端口</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.19%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p1907115310467"><a name="zh-cn_topic_0180960123_p1907115310467"></a><a name="zh-cn_topic_0180960123_p1907115310467"></a>端口为HexaTier的连接端口，建议与数据库端口相同，若相同端口已占用，用户可以配置除0~1023、5000和其他已占用端口之外的任一可用端口。</p>
        <div class="note" id="zh-cn_topic_0180960123_note29071253144613"><a name="zh-cn_topic_0180960123_note29071253144613"></a><a name="zh-cn_topic_0180960123_note29071253144613"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0180960123_p169071653164616"><a name="zh-cn_topic_0180960123_p169071653164616"></a><a name="zh-cn_topic_0180960123_p169071653164616"></a>建议用户为DDM实例的多个连接地址配置相同的代理端口。</p>
        </div></div>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row15907115304617"><td class="cellrowborder" valign="top" width="24.81%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p119073539468"><a name="zh-cn_topic_0180960123_p119073539468"></a><a name="zh-cn_topic_0180960123_p119073539468"></a>状态</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.19%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p49078539462"><a name="zh-cn_topic_0180960123_p49078539462"></a><a name="zh-cn_topic_0180960123_p49078539462"></a>选择下列选项之一：</p>
        <a name="zh-cn_topic_0180960123_ul179071653164618"></a><a name="zh-cn_topic_0180960123_ul179071653164618"></a><ul id="zh-cn_topic_0180960123_ul179071653164618"><li>激活：激活代理。</li><li>禁用：禁用代理。</li><li>旁路：流量将不经过检查直接转发给数据库（不安全）。</li></ul>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row159071753134612"><td class="cellrowborder" valign="top" width="24.81%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p590715354618"><a name="zh-cn_topic_0180960123_p590715354618"></a><a name="zh-cn_topic_0180960123_p590715354618"></a>SSL证书</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.19%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p159071953164620"><a name="zh-cn_topic_0180960123_p159071953164620"></a><a name="zh-cn_topic_0180960123_p159071953164620"></a>DDM不支持SSL连接。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0180960123_row390745315462"><td class="cellrowborder" valign="top" width="24.81%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960123_p09072053164618"><a name="zh-cn_topic_0180960123_p09072053164618"></a><a name="zh-cn_topic_0180960123_p09072053164618"></a>阻止未加密的连接</p>
        </td>
        <td class="cellrowborder" valign="top" width="75.19%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960123_p390717532461"><a name="zh-cn_topic_0180960123_p390717532461"></a><a name="zh-cn_topic_0180960123_p390717532461"></a>未选择该选项，则表示该代理的所有通信均不加密，通信存在安全隐患。</p>
        </td>
        </tr>
        </tbody>
        </table>

    6.  单击“创建“。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >配置受保护数据库的更多信息，请参见[步骤三：添加防护的数据库](zh-cn_topic_0111166540.md)。  

3.  配置数据库防护策略：

    -   配置数据库安全策略，请参见[配置数据库安全策略](zh-cn_topic_0111166347.md)。
    -   配置敏感数据发现策略，请参见[配置敏感数据发现策略](zh-cn_topic_0214274580.md)。
    -   配置数据库防拖库策略，请参见[配置数据库防拖库策略](zh-cn_topic_0142535567.md)。
    -   配置数据库活动监控策略，请参见[配置数据库活动监控策略](zh-cn_topic_0111166467.md)。
    -   配置动态数据脱敏策略，请参见[配置动态数据脱敏策略](zh-cn_topic_0111166389.md)。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >当前不支持创建基于DDM存储过程的数据库防火墙策略和活动监控策略。  


