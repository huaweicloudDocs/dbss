# 配置IP地址对象<a name="ZH-CN_TOPIC_0111166563"></a>

HexaTier支持将外部访问的IP地址设置为对象。用户可以在创建策略规则时，将规则应用于创建的IP地址对象。

用户可以创建IP地址组将多个IP地址和IP范围合并为一个。IP地址对象包含：

-   IP地址
-   IP范围
-   IP地址组

## 操作步骤<a name="zh-cn_topic_0110575003_section7106121115212"></a>

1.  在主菜单上，单击“资源“。
2.  在导航树上，选择“对象定义 \> IP地址管理“。
3.  根据要创建的对象，在导航树上继续选择：
    -   IP地址
    -   IP范围
    -   IP地址组

4.  执行下列操作之一：
    -   创建新的对象

        在命令栏上，单击“新建“。

    -   编辑已有的对象

        找到要编辑的对象，然后单击该行末尾的![](figures/编辑.png)（编辑）。


5.  在工作区，设置以下参数：

    <a name="zh-cn_topic_0110575003_table1452831701319"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0110575003_row1852813175131"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0110575003_p1852871712131"><a name="zh-cn_topic_0110575003_p1852871712131"></a><a name="zh-cn_topic_0110575003_p1852871712131"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0110575003_p85281217151318"><a name="zh-cn_topic_0110575003_p85281217151318"></a><a name="zh-cn_topic_0110575003_p85281217151318"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="65%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0110575003_p95281317111311"><a name="zh-cn_topic_0110575003_p95281317111311"></a><a name="zh-cn_topic_0110575003_p95281317111311"></a>参数说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0110575003_row14528131712135"><td class="cellrowborder" rowspan="5" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p14528117151312"><a name="zh-cn_topic_0110575003_p14528117151312"></a><a name="zh-cn_topic_0110575003_p14528117151312"></a>通用参数</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p125291417131320"><a name="zh-cn_topic_0110575003_p125291417131320"></a><a name="zh-cn_topic_0110575003_p125291417131320"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p3529111716135"><a name="zh-cn_topic_0110575003_p3529111716135"></a><a name="zh-cn_topic_0110575003_p3529111716135"></a>该策略对象的名称。</p>
    <p id="zh-cn_topic_0110575003_p7529417181312"><a name="zh-cn_topic_0110575003_p7529417181312"></a><a name="zh-cn_topic_0110575003_p7529417181312"></a>在设置相应的策略规则时，用户可以选择应用策略规则的对象。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row8529161731313"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p55291717141317"><a name="zh-cn_topic_0110575003_p55291717141317"></a><a name="zh-cn_topic_0110575003_p55291717141317"></a>颜色</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p20529201721314"><a name="zh-cn_topic_0110575003_p20529201721314"></a><a name="zh-cn_topic_0110575003_p20529201721314"></a>在对象列表中，该对象名称将以用户选定的颜色来显示。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row12529161710136"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p175291017131313"><a name="zh-cn_topic_0110575003_p175291017131313"></a><a name="zh-cn_topic_0110575003_p175291017131313"></a>数据库类型</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p14529817151311"><a name="zh-cn_topic_0110575003_p14529817151311"></a><a name="zh-cn_topic_0110575003_p14529817151311"></a>关联该对象的数据库类型，用户也可以不设置，关联所有数据库类型。</p>
    <p id="zh-cn_topic_0110575003_p1552991714137"><a name="zh-cn_topic_0110575003_p1552991714137"></a><a name="zh-cn_topic_0110575003_p1552991714137"></a>选择了数据库类型之后，该对象只会在配置相应数据库类型的策略规则时可选。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row252918173134"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p1852951761315"><a name="zh-cn_topic_0110575003_p1852951761315"></a><a name="zh-cn_topic_0110575003_p1852951761315"></a>代理</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p252941716139"><a name="zh-cn_topic_0110575003_p252941716139"></a><a name="zh-cn_topic_0110575003_p252941716139"></a>关联该IP地址对象的代理，用户也可以不设置，关联所有代理。</p>
    <p id="zh-cn_topic_0110575003_p352961716138"><a name="zh-cn_topic_0110575003_p352961716138"></a><a name="zh-cn_topic_0110575003_p352961716138"></a>选择了代理之后，该对象只会在配置相应代理的策略规则时可选。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row2529151741318"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p17529517181315"><a name="zh-cn_topic_0110575003_p17529517181315"></a><a name="zh-cn_topic_0110575003_p17529517181315"></a>数据库</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p105291617201315"><a name="zh-cn_topic_0110575003_p105291617201315"></a><a name="zh-cn_topic_0110575003_p105291617201315"></a>关联该IP地址对象的数据库，用户也可以不设置，关联所有数据库。</p>
    <p id="zh-cn_topic_0110575003_p1652921751315"><a name="zh-cn_topic_0110575003_p1652921751315"></a><a name="zh-cn_topic_0110575003_p1652921751315"></a>选择了数据库之后，该对象只会在配置相应数据库的策略规则时可选。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row1652917177136"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p252918175137"><a name="zh-cn_topic_0110575003_p252918175137"></a><a name="zh-cn_topic_0110575003_p252918175137"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p8529217171312"><a name="zh-cn_topic_0110575003_p8529217171312"></a><a name="zh-cn_topic_0110575003_p8529217171312"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p11530181761312"><a name="zh-cn_topic_0110575003_p11530181761312"></a><a name="zh-cn_topic_0110575003_p11530181761312"></a>输入IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row653041761320"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p18530617141316"><a name="zh-cn_topic_0110575003_p18530617141316"></a><a name="zh-cn_topic_0110575003_p18530617141316"></a>子网掩码</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p145301817201314"><a name="zh-cn_topic_0110575003_p145301817201314"></a><a name="zh-cn_topic_0110575003_p145301817201314"></a>使用下拉框设置子网掩码。</p>
    <p id="zh-cn_topic_0110575003_p19530161701317"><a name="zh-cn_topic_0110575003_p19530161701317"></a><a name="zh-cn_topic_0110575003_p19530161701317"></a>子网掩码默认值为<span class="parmvalue" id="zh-cn_topic_0110575003_parmvalue11530171761317"><a name="zh-cn_topic_0110575003_parmvalue11530171761317"></a><a name="zh-cn_topic_0110575003_parmvalue11530171761317"></a>“255.255.255.255”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row15530141711313"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p25301717141310"><a name="zh-cn_topic_0110575003_p25301717141310"></a><a name="zh-cn_topic_0110575003_p25301717141310"></a>IP范围</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p4530151741310"><a name="zh-cn_topic_0110575003_p4530151741310"></a><a name="zh-cn_topic_0110575003_p4530151741310"></a>起始IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p85304174139"><a name="zh-cn_topic_0110575003_p85304174139"></a><a name="zh-cn_topic_0110575003_p85304174139"></a>输入IP范围的起始IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row35307174137"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p1530217141320"><a name="zh-cn_topic_0110575003_p1530217141320"></a><a name="zh-cn_topic_0110575003_p1530217141320"></a>结束IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p1653081713133"><a name="zh-cn_topic_0110575003_p1653081713133"></a><a name="zh-cn_topic_0110575003_p1653081713133"></a>输入IP范围的结束IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row165301817191315"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p353041711317"><a name="zh-cn_topic_0110575003_p353041711317"></a><a name="zh-cn_topic_0110575003_p353041711317"></a>IP地址组</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p1653071791314"><a name="zh-cn_topic_0110575003_p1653071791314"></a><a name="zh-cn_topic_0110575003_p1653071791314"></a>可用成员</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p353031716139"><a name="zh-cn_topic_0110575003_p353031716139"></a><a name="zh-cn_topic_0110575003_p353031716139"></a>根据数据库类型、代理、数据库筛选的条件，显示可以添加到对象组的对象名称。</p>
    <p id="zh-cn_topic_0110575003_p4530917201313"><a name="zh-cn_topic_0110575003_p4530917201313"></a><a name="zh-cn_topic_0110575003_p4530917201313"></a>在<span class="parmname" id="zh-cn_topic_0110575003_parmname13530191713136"><a name="zh-cn_topic_0110575003_parmname13530191713136"></a><a name="zh-cn_topic_0110575003_parmname13530191713136"></a>“可用成员”</span>列表中，双击要包含在组中的对象（或选中，然后单击<span class="uicontrol" id="zh-cn_topic_0110575003_uicontrol4531181761316"><a name="zh-cn_topic_0110575003_uicontrol4531181761316"></a><a name="zh-cn_topic_0110575003_uicontrol4531181761316"></a>“添加”</span>），将其添加到<span class="parmname" id="zh-cn_topic_0110575003_parmname653114171135"><a name="zh-cn_topic_0110575003_parmname653114171135"></a><a name="zh-cn_topic_0110575003_parmname653114171135"></a>“当前成员”</span>列表中。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row2531617101318"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p753171761314"><a name="zh-cn_topic_0110575003_p753171761314"></a><a name="zh-cn_topic_0110575003_p753171761314"></a>当前成员</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p1753141712130"><a name="zh-cn_topic_0110575003_p1753141712130"></a><a name="zh-cn_topic_0110575003_p1753141712130"></a>显示已经添加到该对象组的对象名称。</p>
    <p id="zh-cn_topic_0110575003_p35311617111319"><a name="zh-cn_topic_0110575003_p35311617111319"></a><a name="zh-cn_topic_0110575003_p35311617111319"></a>在<span class="parmname" id="zh-cn_topic_0110575003_parmname25311017171314"><a name="zh-cn_topic_0110575003_parmname25311017171314"></a><a name="zh-cn_topic_0110575003_parmname25311017171314"></a>“当前成员”</span>列表中，双击要移除的对象（或选中，然后单击<span class="uicontrol" id="zh-cn_topic_0110575003_uicontrol85311517181320"><a name="zh-cn_topic_0110575003_uicontrol85311517181320"></a><a name="zh-cn_topic_0110575003_uicontrol85311517181320"></a>“移除”</span>），将其从<span class="parmname" id="zh-cn_topic_0110575003_parmname05311217181313"><a name="zh-cn_topic_0110575003_parmname05311217181313"></a><a name="zh-cn_topic_0110575003_parmname05311217181313"></a>“当前成员”</span>列表中删除。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“创建“或“更新“。

