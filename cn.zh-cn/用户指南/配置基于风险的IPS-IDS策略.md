# 配置基于风险的IPS/IDS策略<a name="dbss_01_0041"></a>

用户可基于数据库实际风险，选择应用入侵防御系统（IPS）或入侵检测系统（IDS），并配置对应策略规则，确保用户数据库安全。

## 背景信息<a name="zh-cn_topic_0180960114_section59780192033"></a>

要创建基于风险的IPS/IDS规则，用户可以先创建风险概况（请参见[配置风险概况](#section17892835369)），也可以根据需求来配置风险引擎的各项风险因素评分（请参见[配置风险引擎](#section1856692944012)）。

-   风险概况

    风险概况可根据风险组配置不同的动作行为和日志记录行为，对访问的指定命令或操作进行允许或阻止。基于风险概况，可创建基于风险的IPS/IDS规则。

    风险概况由动作组（风险组）组成，每个组都描述一个不同的风险动作。

    风险概况包括两种设置类型：

    -   动作行为：针对风险组所执行的动作。
    -   日志记录行为：针对风险组进行的日志设置。

    创建风险概况时，可以选择使用“基本模式“或“高级模式“：

    -   “基本模式“下，可以配置服务器、安全和数据库等对象的设置。
    -   “高级模式“下，可以通过单击表中的风险组名称，来查看并指定组里每个动作的行为。


-   风险引擎

    风险引擎定义了对SQL注入攻击的防护，用户可以通过调整每个风险因素的权重评分（1\~100），来配置HexaTier的风险引擎。


## 操作步骤<a name="zh-cn_topic_0180960114_section14742160497"></a>

1.  在HexaTier主菜单上，单击“防火墙“。
2.  根据需要执行以下操作：
    -   创建新的安全规则

        在命令栏，单击“新建“。

    -   编辑已有的安全规则

        找到要编辑的规则，单击该行末尾的![](figures/icon-edit.png)（编辑）。

3.  在“规则类型“中选择“基于风险的IPS/IDS“。
4.  选择应用该防火墙规则的“数据库“和“代理“。
5.  根据需求配置以下参数：

    **表 1**  基于风险的IPS/IDS参数

    <a name="zh-cn_topic_0180960114_tfe5989f468da4275a46ce61cdf97d4a3"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180960114_rd22ba3e866cb48548a3254e83eee3a74"><th class="cellrowborder" valign="top" width="30.080000000000002%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960114_ae250c113a1f649dbb8083fcee454cd37"><a name="zh-cn_topic_0180960114_ae250c113a1f649dbb8083fcee454cd37"></a><a name="zh-cn_topic_0180960114_ae250c113a1f649dbb8083fcee454cd37"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="69.92%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960114_a4afe2321366b4679bda7860631457c53"><a name="zh-cn_topic_0180960114_a4afe2321366b4679bda7860631457c53"></a><a name="zh-cn_topic_0180960114_a4afe2321366b4679bda7860631457c53"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180960114_row4187242911"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a344592f085414dcf82b4c5c2e61882be"><a name="zh-cn_topic_0180960114_a344592f085414dcf82b4c5c2e61882be"></a><a name="zh-cn_topic_0180960114_a344592f085414dcf82b4c5c2e61882be"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_a4da8b42a1ff14e9bac1ef245ce705868"><a name="zh-cn_topic_0180960114_a4da8b42a1ff14e9bac1ef245ce705868"></a><a name="zh-cn_topic_0180960114_a4da8b42a1ff14e9bac1ef245ce705868"></a>该安全策略的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r205a61f77169419ba97ead3660259fd9"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p152471522503"><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p152471522503"></a><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p152471522503"></a>源IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_ab34e3f03a66447138d85e3691e0d3c4c"><a name="zh-cn_topic_0180960114_ab34e3f03a66447138d85e3691e0d3c4c"></a><a name="zh-cn_topic_0180960114_ab34e3f03a66447138d85e3691e0d3c4c"></a>应用该规则的源IP地址，用户可以单击<span class="uicontrol" id="zh-cn_topic_0180960114_u078b79bb45ae4c6ba363f63e2a326fd4"><a name="zh-cn_topic_0180960114_u078b79bb45ae4c6ba363f63e2a326fd4"></a><a name="zh-cn_topic_0180960114_u078b79bb45ae4c6ba363f63e2a326fd4"></a>“新建”</span>来创建新的源IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r5dd575b6956644a0bf479d96380e6d6a"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p425410529501"><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p425410529501"></a><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p425410529501"></a>数据库用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_a76d693ec7bf84f4cbea72b9b0b41e36b"><a name="zh-cn_topic_0180960114_a76d693ec7bf84f4cbea72b9b0b41e36b"></a><a name="zh-cn_topic_0180960114_a76d693ec7bf84f4cbea72b9b0b41e36b"></a>应用该规则的数据库用户，用户可以单击<span class="uicontrol" id="zh-cn_topic_0180960114_u9b7785a2c1c446e7940f866f7fa59467"><a name="zh-cn_topic_0180960114_u9b7785a2c1c446e7940f866f7fa59467"></a><a name="zh-cn_topic_0180960114_u9b7785a2c1c446e7940f866f7fa59467"></a>“新建”</span>来创建新的数据库用户对象。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_row121151710192017"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_ad703537439ff4dbaa56a9926371309ca"><a name="zh-cn_topic_0180960114_ad703537439ff4dbaa56a9926371309ca"></a><a name="zh-cn_topic_0180960114_ad703537439ff4dbaa56a9926371309ca"></a>活动目录用户</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_a6ef8f02512034121ad1d77535b6afa0f"><a name="zh-cn_topic_0180960114_a6ef8f02512034121ad1d77535b6afa0f"></a><a name="zh-cn_topic_0180960114_a6ef8f02512034121ad1d77535b6afa0f"></a>应用该规则的活动目录用户，可以是特定活动目录用户，也可以是用户组。</p>
    <div class="note" id="zh-cn_topic_0180960114_n402f66f692024bc69a23f88de363dac1"><a name="zh-cn_topic_0180960114_n402f66f692024bc69a23f88de363dac1"></a><a name="zh-cn_topic_0180960114_n402f66f692024bc69a23f88de363dac1"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0180960114_zh-cn_topic_0076429722_p5717533161"><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429722_p5717533161"></a><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429722_p5717533161"></a>只有配置了活动目录之后，该参数才会显示，配置活动目录的详细信息，请参见<a href="配置活动目录.md">配置活动目录</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r94e37828316a4ad9ad1a94160b9aa879"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a3bda3fa419964c94a42fd619a98598fa"><a name="zh-cn_topic_0180960114_a3bda3fa419964c94a42fd619a98598fa"></a><a name="zh-cn_topic_0180960114_a3bda3fa419964c94a42fd619a98598fa"></a>应用名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_a7de709b9c9754bbe9e728c4d928adeec"><a name="zh-cn_topic_0180960114_a7de709b9c9754bbe9e728c4d928adeec"></a><a name="zh-cn_topic_0180960114_a7de709b9c9754bbe9e728c4d928adeec"></a>应用该规则的应用名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_re7815b0d48f44fbea9ee3db4ae959645"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_ac5b46c2aec7f48789c0de1822f7fdc6b"><a name="zh-cn_topic_0180960114_ac5b46c2aec7f48789c0de1822f7fdc6b"></a><a name="zh-cn_topic_0180960114_ac5b46c2aec7f48789c0de1822f7fdc6b"></a>计划</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_a8cb574043393442c98150cb6a29715c7"><a name="zh-cn_topic_0180960114_a8cb574043393442c98150cb6a29715c7"></a><a name="zh-cn_topic_0180960114_a8cb574043393442c98150cb6a29715c7"></a>应用该规则的时间计划，用户可以单击<span class="uicontrol" id="zh-cn_topic_0180960114_uede25dff3c854dc7be8bd4452018e941"><a name="zh-cn_topic_0180960114_uede25dff3c854dc7be8bd4452018e941"></a><a name="zh-cn_topic_0180960114_uede25dff3c854dc7be8bd4452018e941"></a>“新建”</span>来创建新的计划。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r3b80820f3ec14a1ba51a3ab4a37908d9"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a8c58a1dc4b474321b262c8a64cca65f6"><a name="zh-cn_topic_0180960114_a8c58a1dc4b474321b262c8a64cca65f6"></a><a name="zh-cn_topic_0180960114_a8c58a1dc4b474321b262c8a64cca65f6"></a>模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_af8f6717355484d4aaa779df103ba7906"><a name="zh-cn_topic_0180960114_af8f6717355484d4aaa779df103ba7906"></a><a name="zh-cn_topic_0180960114_af8f6717355484d4aaa779df103ba7906"></a>选择与SQL注入检测同时执行的任务：</p>
    <a name="zh-cn_topic_0180960114_ua0d3ad0971d840e2ae08bc302555102d"></a><a name="zh-cn_topic_0180960114_ua0d3ad0971d840e2ae08bc302555102d"></a><ul id="zh-cn_topic_0180960114_ua0d3ad0971d840e2ae08bc302555102d"><li>主动防护-IPS：应用入侵防御系统，并阻止与已有风险概况相匹配的查询，或依据配置的风险引擎执行阻止或告警。</li><li>监控-IDS：应用入侵检测系统和已配置的风险概况、风险引擎，并监控查询。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r551d606715a64625af171cf25a702f4c"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_add61289591b1405ab4e41d67939aa06c"><a name="zh-cn_topic_0180960114_add61289591b1405ab4e41d67939aa06c"></a><a name="zh-cn_topic_0180960114_add61289591b1405ab4e41d67939aa06c"></a>风险概况</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p26283323209"><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p26283323209"></a><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p26283323209"></a>根据<span class="parmname" id="zh-cn_topic_0180960114_p6e619d1ed40c44269b06016bcd0be55c"><a name="zh-cn_topic_0180960114_p6e619d1ed40c44269b06016bcd0be55c"></a><a name="zh-cn_topic_0180960114_p6e619d1ed40c44269b06016bcd0be55c"></a>“模式”</span>中的选择，用户可以选择配置了阻止或监控动作的风险概况。配置风险概况，请参见<a href="#section17892835369">配置风险概况</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r0239634953c44bf888b7b4e3ff563c7f"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_acee03fb06df5477f85697ebfe90286f1"><a name="zh-cn_topic_0180960114_acee03fb06df5477f85697ebfe90286f1"></a><a name="zh-cn_topic_0180960114_acee03fb06df5477f85697ebfe90286f1"></a>SQL Injection Detection</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><a name="zh-cn_topic_0180960114_u51416496b5b74614bad33edafd8afbe3"></a><a name="zh-cn_topic_0180960114_u51416496b5b74614bad33edafd8afbe3"></a><ul id="zh-cn_topic_0180960114_u51416496b5b74614bad33edafd8afbe3"><li>如果在<span class="parmname" id="zh-cn_topic_0180960114_pa8f6b9480f534b0680254d08b3c095d3"><a name="zh-cn_topic_0180960114_pa8f6b9480f534b0680254d08b3c095d3"></a><a name="zh-cn_topic_0180960114_pa8f6b9480f534b0680254d08b3c095d3"></a>“模式”</span>中选择了<span class="parmvalue" id="zh-cn_topic_0180960114_p518e53036d12435aa9581f08cde78ccd"><a name="zh-cn_topic_0180960114_p518e53036d12435aa9581f08cde78ccd"></a><a name="zh-cn_topic_0180960114_p518e53036d12435aa9581f08cde78ccd"></a>“主动防护-IPS”</span>，勾选该选项可以阻止SQL注入。</li></ul>
    <a name="zh-cn_topic_0180960114_u43a74faf9d834a6c9a5fe4604712544d"></a><a name="zh-cn_topic_0180960114_u43a74faf9d834a6c9a5fe4604712544d"></a><ul id="zh-cn_topic_0180960114_u43a74faf9d834a6c9a5fe4604712544d"><li>如果在<span class="parmname" id="zh-cn_topic_0180960114_pa72c6609bc0c4beb8d20eaa453947a44"><a name="zh-cn_topic_0180960114_pa72c6609bc0c4beb8d20eaa453947a44"></a><a name="zh-cn_topic_0180960114_pa72c6609bc0c4beb8d20eaa453947a44"></a>“模式”</span>中选择了<span class="parmvalue" id="zh-cn_topic_0180960114_pfabd2693f3cd442c8e933eff9d874656"><a name="zh-cn_topic_0180960114_pfabd2693f3cd442c8e933eff9d874656"></a><a name="zh-cn_topic_0180960114_pfabd2693f3cd442c8e933eff9d874656"></a>“监控-IDS”</span>，勾选该选项可以监控SQL注入。</li></ul>
    <p id="zh-cn_topic_0180960114_addd9e1aec6614e70a0ce8c74696bb4fb"><a name="zh-cn_topic_0180960114_addd9e1aec6614e70a0ce8c74696bb4fb"></a><a name="zh-cn_topic_0180960114_addd9e1aec6614e70a0ce8c74696bb4fb"></a>SQL注入检测以HexaTier内置检测系统（风险引擎）为基础。配置风险引擎，请参见<a href="#section1856692944012">配置风险引擎</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_rf2cdf3561bb64592a644423310c58287"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a0a9c0fad54274fe59ca775da39fc85e0"><a name="zh-cn_topic_0180960114_a0a9c0fad54274fe59ca775da39fc85e0"></a><a name="zh-cn_topic_0180960114_a0a9c0fad54274fe59ca775da39fc85e0"></a>动作</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_ae1d396a625b849f8b44b23c2adee2d00"><a name="zh-cn_topic_0180960114_ae1d396a625b849f8b44b23c2adee2d00"></a><a name="zh-cn_topic_0180960114_ae1d396a625b849f8b44b23c2adee2d00"></a>该规则要采取的动作，该项不需要用户配置：</p>
    <a name="zh-cn_topic_0180960114_u06ee817fd32c44c1a0a6d639351a78dd"></a><a name="zh-cn_topic_0180960114_u06ee817fd32c44c1a0a6d639351a78dd"></a><ul id="zh-cn_topic_0180960114_u06ee817fd32c44c1a0a6d639351a78dd"><li>如果在<span class="parmname" id="zh-cn_topic_0180960114_p5e3aeb7ad92342609a6efd18cae7d39c"><a name="zh-cn_topic_0180960114_p5e3aeb7ad92342609a6efd18cae7d39c"></a><a name="zh-cn_topic_0180960114_p5e3aeb7ad92342609a6efd18cae7d39c"></a>“模式”</span>中选择了<span class="parmvalue" id="zh-cn_topic_0180960114_p18370c540ba54e66b91548d1e00dfe70"><a name="zh-cn_topic_0180960114_p18370c540ba54e66b91548d1e00dfe70"></a><a name="zh-cn_topic_0180960114_p18370c540ba54e66b91548d1e00dfe70"></a>“主动防护-IPS”</span>，则动作始终为阻止。</li><li>如果在<span class="parmname" id="zh-cn_topic_0180960114_p87c6897037834819b12eeb9366fe5271"><a name="zh-cn_topic_0180960114_p87c6897037834819b12eeb9366fe5271"></a><a name="zh-cn_topic_0180960114_p87c6897037834819b12eeb9366fe5271"></a>“模式”</span>中选择了<span class="parmvalue" id="zh-cn_topic_0180960114_pee1382e66a7e4911962039ddd5bfb970"><a name="zh-cn_topic_0180960114_pee1382e66a7e4911962039ddd5bfb970"></a><a name="zh-cn_topic_0180960114_pee1382e66a7e4911962039ddd5bfb970"></a>“监控-IDS”</span>，则动作始终为允许。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r7a4b64b7ff974a4d899179eee9c4e6b2"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a77b929920e32431d854e299ea3d2ea9a"><a name="zh-cn_topic_0180960114_a77b929920e32431d854e299ea3d2ea9a"></a><a name="zh-cn_topic_0180960114_a77b929920e32431d854e299ea3d2ea9a"></a>阻止动作</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><div class="p" id="zh-cn_topic_0180960114_p19486721512"><a name="zh-cn_topic_0180960114_p19486721512"></a><a name="zh-cn_topic_0180960114_p19486721512"></a>如果在<span class="parmname" id="zh-cn_topic_0180960114_parmname1939365011311"><a name="zh-cn_topic_0180960114_parmname1939365011311"></a><a name="zh-cn_topic_0180960114_parmname1939365011311"></a>“模式”</span>中选择了<span class="parmvalue" id="zh-cn_topic_0180960114_parmvalue1339375017310"><a name="zh-cn_topic_0180960114_parmvalue1339375017310"></a><a name="zh-cn_topic_0180960114_parmvalue1339375017310"></a>“主动防护-IPS”</span>，则需要在<span class="parmname" id="zh-cn_topic_0180960114_pee1fd253bd644a728cf65599234d470b"><a name="zh-cn_topic_0180960114_pee1fd253bd644a728cf65599234d470b"></a><a name="zh-cn_topic_0180960114_pee1fd253bd644a728cf65599234d470b"></a>“阻止动作”</span>下拉框中选择以下选项之一：<a name="zh-cn_topic_0180960114_ua758597668a34b8c82a07ea035839099"></a><a name="zh-cn_topic_0180960114_ua758597668a34b8c82a07ea035839099"></a><ul id="zh-cn_topic_0180960114_ua758597668a34b8c82a07ea035839099"><li>返回空结果集</li><li>断开SQL连接</li><li>生成SQL错误</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_rbf6d819f05034744bcf95b18c7a35177"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_acbbe61c42b434fcb974ed974f19ecc1e"><a name="zh-cn_topic_0180960114_acbbe61c42b434fcb974ed974f19ecc1e"></a><a name="zh-cn_topic_0180960114_acbbe61c42b434fcb974ed974f19ecc1e"></a>日志记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_abe92a89344c44400b7029ce68cce23b4"><a name="zh-cn_topic_0180960114_abe92a89344c44400b7029ce68cce23b4"></a><a name="zh-cn_topic_0180960114_abe92a89344c44400b7029ce68cce23b4"></a>选择是否把阻止的查询写入入侵事件日志。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_reb8047df351a4f54ac65cf739438d489"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a10b549ec50be488a90ffd3097a58b97a"><a name="zh-cn_topic_0180960114_a10b549ec50be488a90ffd3097a58b97a"></a><a name="zh-cn_topic_0180960114_a10b549ec50be488a90ffd3097a58b97a"></a>同时生成(SMTP)告警</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_abe020ec20ac04edaa984a7ee5f4f1341"><a name="zh-cn_topic_0180960114_abe020ec20ac04edaa984a7ee5f4f1341"></a><a name="zh-cn_topic_0180960114_abe020ec20ac04edaa984a7ee5f4f1341"></a>如果在日志记录中选择了<span class="parmvalue" id="zh-cn_topic_0180960114_p4719b2b966b74bc09aca8b689b52c242"><a name="zh-cn_topic_0180960114_p4719b2b966b74bc09aca8b689b52c242"></a><a name="zh-cn_topic_0180960114_p4719b2b966b74bc09aca8b689b52c242"></a>“入侵事件”</span>，用户可以勾选<span class="parmvalue" id="zh-cn_topic_0180960114_ped405ff3b3684dde845dd794d054b61b"><a name="zh-cn_topic_0180960114_ped405ff3b3684dde845dd794d054b61b"></a><a name="zh-cn_topic_0180960114_ped405ff3b3684dde845dd794d054b61b"></a>“同时生成（SMTP）告警”</span>来启用告警功能。根据告警中定义的参数，当该规则被激活时都会发送告警。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_rd5fa267115f248078f6c21bba44a66ce"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a1bff20dd060e46d4ad73ed553dde2604"><a name="zh-cn_topic_0180960114_a1bff20dd060e46d4ad73ed553dde2604"></a><a name="zh-cn_topic_0180960114_a1bff20dd060e46d4ad73ed553dde2604"></a>Syslog</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_ab57a43cb9b084a4daafc50155cfd05eb"><a name="zh-cn_topic_0180960114_ab57a43cb9b084a4daafc50155cfd05eb"></a><a name="zh-cn_topic_0180960114_ab57a43cb9b084a4daafc50155cfd05eb"></a>如果在日志记录中选择了<span class="parmvalue" id="zh-cn_topic_0180960114_pa370197a1cd54cfc8995af44e0be5b03"><a name="zh-cn_topic_0180960114_pa370197a1cd54cfc8995af44e0be5b03"></a><a name="zh-cn_topic_0180960114_pa370197a1cd54cfc8995af44e0be5b03"></a>“入侵事件”</span>，用户可以勾选<span class="parmvalue" id="zh-cn_topic_0180960114_pdcf2993d338e4fa2a0a6c75120c388df"><a name="zh-cn_topic_0180960114_pdcf2993d338e4fa2a0a6c75120c388df"></a><a name="zh-cn_topic_0180960114_pdcf2993d338e4fa2a0a6c75120c388df"></a>“Syslog”</span>来启用Syslog。每次激活规则时，会向Syslog服务器发送一条消息。要配置Syslog，请参见<a href="配置Syslog.md">配置Syslog</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r99d04af2b363425689aa653a652323a8"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_ae716838168b24e5c959a708bdc2d8986"><a name="zh-cn_topic_0180960114_ae716838168b24e5c959a708bdc2d8986"></a><a name="zh-cn_topic_0180960114_ae716838168b24e5c959a708bdc2d8986"></a>规则优先级</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p459392214012"><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p459392214012"></a><a name="zh-cn_topic_0180960114_zh-cn_topic_0076429812_p459392214012"></a>本功能用于设置新增策略的优先级。</p>
    <a name="zh-cn_topic_0180960114_ul18427224713"></a><a name="zh-cn_topic_0180960114_ul18427224713"></a><ul id="zh-cn_topic_0180960114_ul18427224713"><li>高：优先应用该新增规则。</li><li>低：最后应用该新增规则。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_row15753128122411"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_p1678591016243"><a name="zh-cn_topic_0180960114_p1678591016243"></a><a name="zh-cn_topic_0180960114_p1678591016243"></a>说明</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_p4785181010244"><a name="zh-cn_topic_0180960114_p4785181010244"></a><a name="zh-cn_topic_0180960114_p4785181010244"></a>该安全规则的备注信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960114_r162729c1fc2e4ed9adca532d57aa04bb"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960114_a56e20803419243379e5bacb01711c821"><a name="zh-cn_topic_0180960114_a56e20803419243379e5bacb01711c821"></a><a name="zh-cn_topic_0180960114_a56e20803419243379e5bacb01711c821"></a>禁用规则</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960114_a056ab46b51c548f289cd796d45dfee47"><a name="zh-cn_topic_0180960114_a056ab46b51c548f289cd796d45dfee47"></a><a name="zh-cn_topic_0180960114_a056ab46b51c548f289cd796d45dfee47"></a>勾选复选框可以禁用该规则。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“创建“或“更新“。

## 配置风险概况<a name="section17892835369"></a>

1.  在HexaTier主菜单上，单击“防火墙“。
2.  在导航树上，选择“风险概况“。
3.  根据需要执行以下操作：
    -   创建新的风险概况

        在命令栏上，单击“新建“。

    -   编辑已有的风险概况

        找到要编辑的风险概况，然后单击行末尾的![](figures/icon-edit.png)（编辑）。

4.  在工作区中，输入“风险概况名称“和“描述“。
5.  在“数据库类型“下拉框中选择数据库类型：
    -   MySQL
    -   MS-SQL

6.  工作区以“基本模式“显示，用户可以单击“高级模式“来显示高级命令。

    **图 1**  高级模式选择<a name="zh-cn_topic_0180960110_fig15378139175420"></a>  
    ![](figures/高级模式选择.png "高级模式选择")

7.  在“动作行为“列中，为每个组选择下列动作行为：

    **表 2**  动作行为说明

    <a name="zh-cn_topic_0180960110_table73115491545"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180960110_row93214497540"><th class="cellrowborder" valign="top" width="26.46%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960110_p1732144945419"><a name="zh-cn_topic_0180960110_p1732144945419"></a><a name="zh-cn_topic_0180960110_p1732144945419"></a>动作行为名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="73.54%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960110_p33210498549"><a name="zh-cn_topic_0180960110_p33210498549"></a><a name="zh-cn_topic_0180960110_p33210498549"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180960110_row13321349105419"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p5321049185419"><a name="zh-cn_topic_0180960110_p5321049185419"></a><a name="zh-cn_topic_0180960110_p5321049185419"></a>允许</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p6321649155414"><a name="zh-cn_topic_0180960110_p6321649155414"></a><a name="zh-cn_topic_0180960110_p6321649155414"></a>允许该组的所有动作。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960110_row63294915414"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p1532104935419"><a name="zh-cn_topic_0180960110_p1532104935419"></a><a name="zh-cn_topic_0180960110_p1532104935419"></a>阻止</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p2321949105411"><a name="zh-cn_topic_0180960110_p2321949105411"></a><a name="zh-cn_topic_0180960110_p2321949105411"></a>阻止该组的所有动作。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960110_row93211496547"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p33224910541"><a name="zh-cn_topic_0180960110_p33224910541"></a><a name="zh-cn_topic_0180960110_p33224910541"></a>无</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p932104911547"><a name="zh-cn_topic_0180960110_p932104911547"></a><a name="zh-cn_topic_0180960110_p932104911547"></a>忽略该组的所有动作。此选项通过不处理查询来节省资源。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960110_row143224935412"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p12321249105412"><a name="zh-cn_topic_0180960110_p12321249105412"></a><a name="zh-cn_topic_0180960110_p12321249105412"></a>自定义</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p16404173917616"><a name="zh-cn_topic_0180960110_p16404173917616"></a><a name="zh-cn_topic_0180960110_p16404173917616"></a>在基本模式下，可以对组中的不同对象制定不同行为。</p>
    <p id="zh-cn_topic_0180960110_p6328495540"><a name="zh-cn_topic_0180960110_p6328495540"></a><a name="zh-cn_topic_0180960110_p6328495540"></a>如果选择高级模式，则允许为组中的每个动作指定不同的行为。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960110_row1332194917540"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p2325490548"><a name="zh-cn_topic_0180960110_p2325490548"></a><a name="zh-cn_topic_0180960110_p2325490548"></a>默认</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.54%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p113224995410"><a name="zh-cn_topic_0180960110_p113224995410"></a><a name="zh-cn_topic_0180960110_p113224995410"></a>使用IPS或IDS策略中配置的默认动作。</p>
    </td>
    </tr>
    </tbody>
    </table>

8.  在“日志记录行为“列中，为每个组选择下列日志记录行为：

    **表 3**  日志记录行为说明

    <a name="zh-cn_topic_0180960110_table24071645135514"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180960110_row3408204515515"><th class="cellrowborder" valign="top" width="26.83%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960110_p640874585513"><a name="zh-cn_topic_0180960110_p640874585513"></a><a name="zh-cn_topic_0180960110_p640874585513"></a>日志记录行为名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="73.17%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960110_p10408154545510"><a name="zh-cn_topic_0180960110_p10408154545510"></a><a name="zh-cn_topic_0180960110_p10408154545510"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180960110_row6408174516559"><td class="cellrowborder" valign="top" width="26.83%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p1408104525514"><a name="zh-cn_topic_0180960110_p1408104525514"></a><a name="zh-cn_topic_0180960110_p1408104525514"></a>启用</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.17%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p54081645135513"><a name="zh-cn_topic_0180960110_p54081645135513"></a><a name="zh-cn_topic_0180960110_p54081645135513"></a>启用该组所有动作的日志记录。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960110_row164081345205514"><td class="cellrowborder" valign="top" width="26.83%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p540804512555"><a name="zh-cn_topic_0180960110_p540804512555"></a><a name="zh-cn_topic_0180960110_p540804512555"></a>禁用</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.17%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p140824518553"><a name="zh-cn_topic_0180960110_p140824518553"></a><a name="zh-cn_topic_0180960110_p140824518553"></a>禁用该组所有动作的日志记录。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960110_row94087456554"><td class="cellrowborder" valign="top" width="26.83%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p194081745185514"><a name="zh-cn_topic_0180960110_p194081745185514"></a><a name="zh-cn_topic_0180960110_p194081745185514"></a>自定义</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.17%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p17846204219612"><a name="zh-cn_topic_0180960110_p17846204219612"></a><a name="zh-cn_topic_0180960110_p17846204219612"></a>在基本模式下，可以对组中的不同对象制定不同的日志记录行为。</p>
    <p id="zh-cn_topic_0180960110_p1940894516555"><a name="zh-cn_topic_0180960110_p1940894516555"></a><a name="zh-cn_topic_0180960110_p1940894516555"></a>如果选择高级模式，则允许为组中的每个动作指定不同的日志记录行为。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960110_row740814595511"><td class="cellrowborder" valign="top" width="26.83%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960110_p174081945155516"><a name="zh-cn_topic_0180960110_p174081945155516"></a><a name="zh-cn_topic_0180960110_p174081945155516"></a>默认</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.17%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960110_p20408104512559"><a name="zh-cn_topic_0180960110_p20408104512559"></a><a name="zh-cn_topic_0180960110_p20408104512559"></a>使用IPS或IDS策略中配置的默认日志行为。</p>
    </td>
    </tr>
    </tbody>
    </table>

9.  单击“创建“或“更新“。

## 配置风险引擎<a name="section1856692944012"></a>

1.  在HexaTier主菜单上，单击“防火墙“。
2.  在导航树上，选择“风险概况 \> 风险引擎“。
3.  根据需要，设置以下风险因素的权重评分（1\~100）：
    -   警告级别的风险评分
    -   阻止级别的风险评分
    -   查询语句中包含与SQL注释相关的风险因素评分。
    -   语句中包含“OR”相关的风险因素评分
    -   语句中包含“UNION”相关的风险因素评分
    -   语句中包含参数比较相关的风险因素评分。比如：1=1
    -   语句中包含恒成立语句的风险因素评分，比如：Select \* from XXX where 1
    -   语句中包含空密码的风险因素评分。比如：select \* from users where password=''，密码字段名需要为以下任一：pass/pwd/passwd/password
    -   语句被分号（;）分割为多个语句的风险因素评分
    -   暴力破解数据库内容的SQL命令的风险因素评分
    -   使用敏感函数、存储过程或表相关的风险因素评分

4.  在“禁用存储过程和函数的风险评估“中，选择是否禁用该项：
    -   否：启用该风险评估
    -   是：禁用该风险评估

5.  单击“保存“。

>![](public_sys-resources/icon-note.gif) **说明：** 
>若要恢复风险引擎各参数为原始设置，请单击“重置“。

