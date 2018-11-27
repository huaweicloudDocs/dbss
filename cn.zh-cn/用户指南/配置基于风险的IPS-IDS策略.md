# 配置基于风险的IPS/IDS策略<a name="ZH-CN_TOPIC_0111166557"></a>

用户可基于数据库实际风险，选择应用入侵防御系统（IPS）或入侵检测系统（IDS），并配置对应策略规则，确保用户数据库安全。

基于风险的IPS/IDS规则支持SQL注入检测和风险概况的组合使用。

要创建基于风险的IPS/IDS规则，用户可以先创建风险概况（请参见[配置风险概况](配置风险概况.md#ZH-CN_TOPIC_0111166352)），也可以根据需求来配置风险引擎的各项风险因素评分（请参见[配置风险引擎](配置风险引擎.md#ZH-CN_TOPIC_0111166556)）。

## 操作过程<a name="zh-cn_topic_0110574903_section14742160497"></a>

1.  在HexaTier主菜单上，单击“防火墙“。
2.  根据需要执行以下操作：
    -   创建新的安全规则

        在命令栏，单击“新建“。

    -   编辑已有的安全规则

        找到要编辑的规则，单击该行末尾的![](figures/编辑.png)（编辑）。


3.  在“规则类型“中选择“基于风险的IPS/IDS“。
4.  选择应用该防火墙规则的“数据库“和“代理“。
5.  根据需求配置以下参数：

    **表 1**  基于风险的IPS/IDS参数

    <a name="zh-cn_topic_0110574903_tfe5989f468da4275a46ce61cdf97d4a3"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0110574903_rd22ba3e866cb48548a3254e83eee3a74"><th class="cellrowborder" valign="top" width="30.080000000000002%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0110574903_ae250c113a1f649dbb8083fcee454cd37"><a name="zh-cn_topic_0110574903_ae250c113a1f649dbb8083fcee454cd37"></a><a name="zh-cn_topic_0110574903_ae250c113a1f649dbb8083fcee454cd37"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="69.92%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0110574903_a4afe2321366b4679bda7860631457c53"><a name="zh-cn_topic_0110574903_a4afe2321366b4679bda7860631457c53"></a><a name="zh-cn_topic_0110574903_a4afe2321366b4679bda7860631457c53"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0110574903_row4187242911"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a344592f085414dcf82b4c5c2e61882be"><a name="zh-cn_topic_0110574903_a344592f085414dcf82b4c5c2e61882be"></a><a name="zh-cn_topic_0110574903_a344592f085414dcf82b4c5c2e61882be"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_a4da8b42a1ff14e9bac1ef245ce705868"><a name="zh-cn_topic_0110574903_a4da8b42a1ff14e9bac1ef245ce705868"></a><a name="zh-cn_topic_0110574903_a4da8b42a1ff14e9bac1ef245ce705868"></a>该安全策略的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r205a61f77169419ba97ead3660259fd9"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p152471522503"><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p152471522503"></a><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p152471522503"></a>源IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_ab34e3f03a66447138d85e3691e0d3c4c"><a name="zh-cn_topic_0110574903_ab34e3f03a66447138d85e3691e0d3c4c"></a><a name="zh-cn_topic_0110574903_ab34e3f03a66447138d85e3691e0d3c4c"></a>应用该规则的源IP地址，用户可以单击<span class="uicontrol" id="zh-cn_topic_0110574903_u078b79bb45ae4c6ba363f63e2a326fd4"><a name="zh-cn_topic_0110574903_u078b79bb45ae4c6ba363f63e2a326fd4"></a><a name="zh-cn_topic_0110574903_u078b79bb45ae4c6ba363f63e2a326fd4"></a><b>新建</b></span>来创建新的源IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r5dd575b6956644a0bf479d96380e6d6a"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p425410529501"><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p425410529501"></a><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p425410529501"></a>数据库用户</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_a76d693ec7bf84f4cbea72b9b0b41e36b"><a name="zh-cn_topic_0110574903_a76d693ec7bf84f4cbea72b9b0b41e36b"></a><a name="zh-cn_topic_0110574903_a76d693ec7bf84f4cbea72b9b0b41e36b"></a>应用该规则的数据库用户，用户可以单击<span class="uicontrol" id="zh-cn_topic_0110574903_u9b7785a2c1c446e7940f866f7fa59467"><a name="zh-cn_topic_0110574903_u9b7785a2c1c446e7940f866f7fa59467"></a><a name="zh-cn_topic_0110574903_u9b7785a2c1c446e7940f866f7fa59467"></a><b>新建</b></span>来创建新的数据库用户对象。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_row121151710192017"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_ad703537439ff4dbaa56a9926371309ca"><a name="zh-cn_topic_0110574903_ad703537439ff4dbaa56a9926371309ca"></a><a name="zh-cn_topic_0110574903_ad703537439ff4dbaa56a9926371309ca"></a>活动目录用户</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_a6ef8f02512034121ad1d77535b6afa0f"><a name="zh-cn_topic_0110574903_a6ef8f02512034121ad1d77535b6afa0f"></a><a name="zh-cn_topic_0110574903_a6ef8f02512034121ad1d77535b6afa0f"></a>应用该规则的活动目录用户，可以是特定活动目录用户，也可以是用户组。</p>
    <div class="note" id="zh-cn_topic_0110574903_n402f66f692024bc69a23f88de363dac1"><a name="zh-cn_topic_0110574903_n402f66f692024bc69a23f88de363dac1"></a><a name="zh-cn_topic_0110574903_n402f66f692024bc69a23f88de363dac1"></a><span class="notetitle"> NOTE: </span><div class="notebody"><p id="zh-cn_topic_0110574903_zh-cn_topic_0076429722_p5717533161"><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429722_p5717533161"></a><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429722_p5717533161"></a>只有配置了活动目录之后，该参数才会显示，配置活动目录的详细信息，请参见<a href="活动目录简介.md#ZH-CN_TOPIC_0111166491">配置活动目录</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r94e37828316a4ad9ad1a94160b9aa879"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a3bda3fa419964c94a42fd619a98598fa"><a name="zh-cn_topic_0110574903_a3bda3fa419964c94a42fd619a98598fa"></a><a name="zh-cn_topic_0110574903_a3bda3fa419964c94a42fd619a98598fa"></a>应用名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_a7de709b9c9754bbe9e728c4d928adeec"><a name="zh-cn_topic_0110574903_a7de709b9c9754bbe9e728c4d928adeec"></a><a name="zh-cn_topic_0110574903_a7de709b9c9754bbe9e728c4d928adeec"></a>应用该规则的应用名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_re7815b0d48f44fbea9ee3db4ae959645"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_ac5b46c2aec7f48789c0de1822f7fdc6b"><a name="zh-cn_topic_0110574903_ac5b46c2aec7f48789c0de1822f7fdc6b"></a><a name="zh-cn_topic_0110574903_ac5b46c2aec7f48789c0de1822f7fdc6b"></a>计划</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_a8cb574043393442c98150cb6a29715c7"><a name="zh-cn_topic_0110574903_a8cb574043393442c98150cb6a29715c7"></a><a name="zh-cn_topic_0110574903_a8cb574043393442c98150cb6a29715c7"></a>应用该规则的时间计划，用户可以单击<span class="uicontrol" id="zh-cn_topic_0110574903_uede25dff3c854dc7be8bd4452018e941"><a name="zh-cn_topic_0110574903_uede25dff3c854dc7be8bd4452018e941"></a><a name="zh-cn_topic_0110574903_uede25dff3c854dc7be8bd4452018e941"></a><b>新建</b></span>来创建新的计划。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r3b80820f3ec14a1ba51a3ab4a37908d9"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a8c58a1dc4b474321b262c8a64cca65f6"><a name="zh-cn_topic_0110574903_a8c58a1dc4b474321b262c8a64cca65f6"></a><a name="zh-cn_topic_0110574903_a8c58a1dc4b474321b262c8a64cca65f6"></a>模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_af8f6717355484d4aaa779df103ba7906"><a name="zh-cn_topic_0110574903_af8f6717355484d4aaa779df103ba7906"></a><a name="zh-cn_topic_0110574903_af8f6717355484d4aaa779df103ba7906"></a>选择与SQL注入检测同时执行的任务：</p>
    <a name="zh-cn_topic_0110574903_ua0d3ad0971d840e2ae08bc302555102d"></a><a name="zh-cn_topic_0110574903_ua0d3ad0971d840e2ae08bc302555102d"></a><ul id="zh-cn_topic_0110574903_ua0d3ad0971d840e2ae08bc302555102d"><li>主动防护-IPS：应用入侵防御系统，并阻止与已有风险概况相匹配的查询，或依据配置的风险引擎执行阻止或告警。</li><li>监控-IDS：应用入侵检测系统和已配置的风险概况、风险引擎，并监控查询。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r551d606715a64625af171cf25a702f4c"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_add61289591b1405ab4e41d67939aa06c"><a name="zh-cn_topic_0110574903_add61289591b1405ab4e41d67939aa06c"></a><a name="zh-cn_topic_0110574903_add61289591b1405ab4e41d67939aa06c"></a>风险概况</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p26283323209"><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p26283323209"></a><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p26283323209"></a>根据<span class="parmname" id="zh-cn_topic_0110574903_p6e619d1ed40c44269b06016bcd0be55c"><a name="zh-cn_topic_0110574903_p6e619d1ed40c44269b06016bcd0be55c"></a><a name="zh-cn_topic_0110574903_p6e619d1ed40c44269b06016bcd0be55c"></a><b>模式</b></span>中的选择，用户可以选择配置了阻止或监控动作的风险概况。配置风险概况，请参见<a href="配置风险概况.md#ZH-CN_TOPIC_0111166352">配置风险概况</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r0239634953c44bf888b7b4e3ff563c7f"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_acee03fb06df5477f85697ebfe90286f1"><a name="zh-cn_topic_0110574903_acee03fb06df5477f85697ebfe90286f1"></a><a name="zh-cn_topic_0110574903_acee03fb06df5477f85697ebfe90286f1"></a>SQL Injection Detection</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><a name="zh-cn_topic_0110574903_u51416496b5b74614bad33edafd8afbe3"></a><a name="zh-cn_topic_0110574903_u51416496b5b74614bad33edafd8afbe3"></a><ul id="zh-cn_topic_0110574903_u51416496b5b74614bad33edafd8afbe3"><li>如果在<span class="parmname" id="zh-cn_topic_0110574903_pa8f6b9480f534b0680254d08b3c095d3"><a name="zh-cn_topic_0110574903_pa8f6b9480f534b0680254d08b3c095d3"></a><a name="zh-cn_topic_0110574903_pa8f6b9480f534b0680254d08b3c095d3"></a><b>模式</b></span>中选择了<span class="parmvalue" id="zh-cn_topic_0110574903_p518e53036d12435aa9581f08cde78ccd"><a name="zh-cn_topic_0110574903_p518e53036d12435aa9581f08cde78ccd"></a><a name="zh-cn_topic_0110574903_p518e53036d12435aa9581f08cde78ccd"></a><b>主动防护-IPS</b></span>，勾选该选项可以阻止SQL注入。</li></ul>
    <a name="zh-cn_topic_0110574903_u43a74faf9d834a6c9a5fe4604712544d"></a><a name="zh-cn_topic_0110574903_u43a74faf9d834a6c9a5fe4604712544d"></a><ul id="zh-cn_topic_0110574903_u43a74faf9d834a6c9a5fe4604712544d"><li>如果在<span class="parmname" id="zh-cn_topic_0110574903_pa72c6609bc0c4beb8d20eaa453947a44"><a name="zh-cn_topic_0110574903_pa72c6609bc0c4beb8d20eaa453947a44"></a><a name="zh-cn_topic_0110574903_pa72c6609bc0c4beb8d20eaa453947a44"></a><b>模式</b></span>中选择了<span class="parmvalue" id="zh-cn_topic_0110574903_pfabd2693f3cd442c8e933eff9d874656"><a name="zh-cn_topic_0110574903_pfabd2693f3cd442c8e933eff9d874656"></a><a name="zh-cn_topic_0110574903_pfabd2693f3cd442c8e933eff9d874656"></a><b>监控-IDS</b></span>，勾选该选项可以监控SQL注入。</li></ul>
    <p id="zh-cn_topic_0110574903_addd9e1aec6614e70a0ce8c74696bb4fb"><a name="zh-cn_topic_0110574903_addd9e1aec6614e70a0ce8c74696bb4fb"></a><a name="zh-cn_topic_0110574903_addd9e1aec6614e70a0ce8c74696bb4fb"></a>SQL注入检测以HexaTier内置检测系统（风险引擎）为基础。配置风险引擎，请参见<a href="配置风险引擎.md#ZH-CN_TOPIC_0111166556">配置风险引擎</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_rf2cdf3561bb64592a644423310c58287"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a0a9c0fad54274fe59ca775da39fc85e0"><a name="zh-cn_topic_0110574903_a0a9c0fad54274fe59ca775da39fc85e0"></a><a name="zh-cn_topic_0110574903_a0a9c0fad54274fe59ca775da39fc85e0"></a>动作</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_ae1d396a625b849f8b44b23c2adee2d00"><a name="zh-cn_topic_0110574903_ae1d396a625b849f8b44b23c2adee2d00"></a><a name="zh-cn_topic_0110574903_ae1d396a625b849f8b44b23c2adee2d00"></a>该规则要采取的动作，该项不需要用户配置：</p>
    <a name="zh-cn_topic_0110574903_u06ee817fd32c44c1a0a6d639351a78dd"></a><a name="zh-cn_topic_0110574903_u06ee817fd32c44c1a0a6d639351a78dd"></a><ul id="zh-cn_topic_0110574903_u06ee817fd32c44c1a0a6d639351a78dd"><li>如果在<span class="parmname" id="zh-cn_topic_0110574903_p5e3aeb7ad92342609a6efd18cae7d39c"><a name="zh-cn_topic_0110574903_p5e3aeb7ad92342609a6efd18cae7d39c"></a><a name="zh-cn_topic_0110574903_p5e3aeb7ad92342609a6efd18cae7d39c"></a><b>模式</b></span>中选择了<span class="parmvalue" id="zh-cn_topic_0110574903_p18370c540ba54e66b91548d1e00dfe70"><a name="zh-cn_topic_0110574903_p18370c540ba54e66b91548d1e00dfe70"></a><a name="zh-cn_topic_0110574903_p18370c540ba54e66b91548d1e00dfe70"></a><b>主动防护-IPS</b></span>，则动作始终为阻止。</li><li>如果在<span class="parmname" id="zh-cn_topic_0110574903_p87c6897037834819b12eeb9366fe5271"><a name="zh-cn_topic_0110574903_p87c6897037834819b12eeb9366fe5271"></a><a name="zh-cn_topic_0110574903_p87c6897037834819b12eeb9366fe5271"></a><b>模式</b></span>中选择了<span class="parmvalue" id="zh-cn_topic_0110574903_pee1382e66a7e4911962039ddd5bfb970"><a name="zh-cn_topic_0110574903_pee1382e66a7e4911962039ddd5bfb970"></a><a name="zh-cn_topic_0110574903_pee1382e66a7e4911962039ddd5bfb970"></a><b>监控-IDS</b></span>，则动作始终为允许。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r7a4b64b7ff974a4d899179eee9c4e6b2"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a77b929920e32431d854e299ea3d2ea9a"><a name="zh-cn_topic_0110574903_a77b929920e32431d854e299ea3d2ea9a"></a><a name="zh-cn_topic_0110574903_a77b929920e32431d854e299ea3d2ea9a"></a>阻止动作</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><div class="p" id="zh-cn_topic_0110574903_p19486721512"><a name="zh-cn_topic_0110574903_p19486721512"></a><a name="zh-cn_topic_0110574903_p19486721512"></a>如果在<span class="parmname" id="zh-cn_topic_0110574903_p09ee47e9dd274574ba451769a7adc8e9"><a name="zh-cn_topic_0110574903_p09ee47e9dd274574ba451769a7adc8e9"></a><a name="zh-cn_topic_0110574903_p09ee47e9dd274574ba451769a7adc8e9"></a><b>动作</b></span>下拉框中选择了<span class="parmvalue" id="zh-cn_topic_0110574903_pe9bde0d00e474308920bb65e84dcd6c6"><a name="zh-cn_topic_0110574903_pe9bde0d00e474308920bb65e84dcd6c6"></a><a name="zh-cn_topic_0110574903_pe9bde0d00e474308920bb65e84dcd6c6"></a><b>阻止</b></span>，则需要在<span class="parmname" id="zh-cn_topic_0110574903_pee1fd253bd644a728cf65599234d470b"><a name="zh-cn_topic_0110574903_pee1fd253bd644a728cf65599234d470b"></a><a name="zh-cn_topic_0110574903_pee1fd253bd644a728cf65599234d470b"></a><b>阻止动作</b></span>下拉框中选择以下选项之一：<a name="zh-cn_topic_0110574903_ua758597668a34b8c82a07ea035839099"></a><a name="zh-cn_topic_0110574903_ua758597668a34b8c82a07ea035839099"></a><ul id="zh-cn_topic_0110574903_ua758597668a34b8c82a07ea035839099"><li>返回空结果集</li><li>断开SQL连接</li><li>生成SQL错误</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_rbf6d819f05034744bcf95b18c7a35177"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_acbbe61c42b434fcb974ed974f19ecc1e"><a name="zh-cn_topic_0110574903_acbbe61c42b434fcb974ed974f19ecc1e"></a><a name="zh-cn_topic_0110574903_acbbe61c42b434fcb974ed974f19ecc1e"></a>日志记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_abe92a89344c44400b7029ce68cce23b4"><a name="zh-cn_topic_0110574903_abe92a89344c44400b7029ce68cce23b4"></a><a name="zh-cn_topic_0110574903_abe92a89344c44400b7029ce68cce23b4"></a>选择是否把阻止的查询写入入侵事件日志。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_reb8047df351a4f54ac65cf739438d489"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a10b549ec50be488a90ffd3097a58b97a"><a name="zh-cn_topic_0110574903_a10b549ec50be488a90ffd3097a58b97a"></a><a name="zh-cn_topic_0110574903_a10b549ec50be488a90ffd3097a58b97a"></a>告警（SMTP）</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_abe020ec20ac04edaa984a7ee5f4f1341"><a name="zh-cn_topic_0110574903_abe020ec20ac04edaa984a7ee5f4f1341"></a><a name="zh-cn_topic_0110574903_abe020ec20ac04edaa984a7ee5f4f1341"></a>如果在日志记录中选择了<span class="parmvalue" id="zh-cn_topic_0110574903_p4719b2b966b74bc09aca8b689b52c242"><a name="zh-cn_topic_0110574903_p4719b2b966b74bc09aca8b689b52c242"></a><a name="zh-cn_topic_0110574903_p4719b2b966b74bc09aca8b689b52c242"></a><b>入侵事件</b></span>，用户可以勾选<span class="parmvalue" id="zh-cn_topic_0110574903_ped405ff3b3684dde845dd794d054b61b"><a name="zh-cn_topic_0110574903_ped405ff3b3684dde845dd794d054b61b"></a><a name="zh-cn_topic_0110574903_ped405ff3b3684dde845dd794d054b61b"></a><b><span id="zh-cn_topic_0110574903_text18206125013232"><a name="zh-cn_topic_0110574903_text18206125013232"></a><a name="zh-cn_topic_0110574903_text18206125013232"></a>告警（SMTP）</span></b></span>来启用告警功能。根据告警中定义的参数，当该规则被激活时都会发送告警。要配置告警功能，请参见<a href="告警信息简介.md#ZH-CN_TOPIC_0111166388">配置告警信息</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_rd5fa267115f248078f6c21bba44a66ce"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a1bff20dd060e46d4ad73ed553dde2604"><a name="zh-cn_topic_0110574903_a1bff20dd060e46d4ad73ed553dde2604"></a><a name="zh-cn_topic_0110574903_a1bff20dd060e46d4ad73ed553dde2604"></a>Syslog</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_ab57a43cb9b084a4daafc50155cfd05eb"><a name="zh-cn_topic_0110574903_ab57a43cb9b084a4daafc50155cfd05eb"></a><a name="zh-cn_topic_0110574903_ab57a43cb9b084a4daafc50155cfd05eb"></a>如果在日志记录中选择了<span class="parmvalue" id="zh-cn_topic_0110574903_pa370197a1cd54cfc8995af44e0be5b03"><a name="zh-cn_topic_0110574903_pa370197a1cd54cfc8995af44e0be5b03"></a><a name="zh-cn_topic_0110574903_pa370197a1cd54cfc8995af44e0be5b03"></a><b>入侵事件</b></span>，用户可以勾选<span class="parmvalue" id="zh-cn_topic_0110574903_pdcf2993d338e4fa2a0a6c75120c388df"><a name="zh-cn_topic_0110574903_pdcf2993d338e4fa2a0a6c75120c388df"></a><a name="zh-cn_topic_0110574903_pdcf2993d338e4fa2a0a6c75120c388df"></a><b>Syslog</b></span>来启用Syslog。每次激活规则时，会向Syslog服务器发送一条消息。要配置Syslog，请参见<a href="配置Syslog.md#ZH-CN_TOPIC_0111166474">配置Syslog</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r99d04af2b363425689aa653a652323a8"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_ae716838168b24e5c959a708bdc2d8986"><a name="zh-cn_topic_0110574903_ae716838168b24e5c959a708bdc2d8986"></a><a name="zh-cn_topic_0110574903_ae716838168b24e5c959a708bdc2d8986"></a>规则优先级</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p459392214012"><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p459392214012"></a><a name="zh-cn_topic_0110574903_zh-cn_topic_0076429812_p459392214012"></a>本功能用于设置新增策略的优先级。</p>
    <a name="zh-cn_topic_0110574903_ul18427224713"></a><a name="zh-cn_topic_0110574903_ul18427224713"></a><ul id="zh-cn_topic_0110574903_ul18427224713"><li>高：优先应用该新增规则。</li><li>低：最后应用该新增规则。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_row15753128122411"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_p1678591016243"><a name="zh-cn_topic_0110574903_p1678591016243"></a><a name="zh-cn_topic_0110574903_p1678591016243"></a>说明</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_p4785181010244"><a name="zh-cn_topic_0110574903_p4785181010244"></a><a name="zh-cn_topic_0110574903_p4785181010244"></a>该安全规则的备注信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110574903_r162729c1fc2e4ed9adca532d57aa04bb"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0110574903_a56e20803419243379e5bacb01711c821"><a name="zh-cn_topic_0110574903_a56e20803419243379e5bacb01711c821"></a><a name="zh-cn_topic_0110574903_a56e20803419243379e5bacb01711c821"></a>禁用规则</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0110574903_a056ab46b51c548f289cd796d45dfee47"><a name="zh-cn_topic_0110574903_a056ab46b51c548f289cd796d45dfee47"></a><a name="zh-cn_topic_0110574903_a056ab46b51c548f289cd796d45dfee47"></a>勾选复选框可以禁用该规则。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“创建“或“更新“。

