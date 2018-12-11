# 配置IP地址对象<a name="ZH-CN_TOPIC_0111166563"></a>

HexaTier支持将外部访问的IP地址设置为对象。用户可以在创建策略规则时，将规则应用于创建的IP地址对象。

## 操作场景<a name="zh-cn_topic_0110575003_section27234667153559"></a>

该任务指导用户创建或编辑IP地址对象。

用户也可以创建IP地址组将多个IP地址对象合并为一个。

计划对象包括：

-   IP地址
-   IP范围
-   IP地址组

## 操作过程<a name="zh-cn_topic_0110575003_section7106121115212"></a>

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

    <a name="zh-cn_topic_0110575003_table1169941314365"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0110575003_row870091310364"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0110575003_p1270011316363"><a name="zh-cn_topic_0110575003_p1270011316363"></a><a name="zh-cn_topic_0110575003_p1270011316363"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0110575003_p11700181318369"><a name="zh-cn_topic_0110575003_p11700181318369"></a><a name="zh-cn_topic_0110575003_p11700181318369"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="65%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0110575003_p197001713163620"><a name="zh-cn_topic_0110575003_p197001713163620"></a><a name="zh-cn_topic_0110575003_p197001713163620"></a>参数说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0110575003_row670061313363"><td class="cellrowborder" rowspan="5" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p270012135361"><a name="zh-cn_topic_0110575003_p270012135361"></a><a name="zh-cn_topic_0110575003_p270012135361"></a>通用参数</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p10701151373619"><a name="zh-cn_topic_0110575003_p10701151373619"></a><a name="zh-cn_topic_0110575003_p10701151373619"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p13747164310519"><a name="zh-cn_topic_0110575003_p13747164310519"></a><a name="zh-cn_topic_0110575003_p13747164310519"></a>该策略对象的名称。</p>
    <p id="zh-cn_topic_0110575003_p067265111557"><a name="zh-cn_topic_0110575003_p067265111557"></a><a name="zh-cn_topic_0110575003_p067265111557"></a>在设置相应的策略规则时，用户可以选择应用策略规则的对象。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row177011413113618"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p117011513113611"><a name="zh-cn_topic_0110575003_p117011513113611"></a><a name="zh-cn_topic_0110575003_p117011513113611"></a>颜色</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p8701813193619"><a name="zh-cn_topic_0110575003_p8701813193619"></a><a name="zh-cn_topic_0110575003_p8701813193619"></a>在对象列表中，该对象名称将以用户选定的颜色来显示。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row2701413173610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p870131373615"><a name="zh-cn_topic_0110575003_p870131373615"></a><a name="zh-cn_topic_0110575003_p870131373615"></a>数据库类型</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p1167210513559"><a name="zh-cn_topic_0110575003_p1167210513559"></a><a name="zh-cn_topic_0110575003_p1167210513559"></a>关联该对象的数据库类型，用户也可以不设置，关联所有数据库类型。</p>
    <p id="zh-cn_topic_0110575003_p165722036105918"><a name="zh-cn_topic_0110575003_p165722036105918"></a><a name="zh-cn_topic_0110575003_p165722036105918"></a>选择了数据库类型之后，该对象只会在配置相应数据库类型的策略规则时可选。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row67011313153610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p570121312360"><a name="zh-cn_topic_0110575003_p570121312360"></a><a name="zh-cn_topic_0110575003_p570121312360"></a>代理</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p548514121007"><a name="zh-cn_topic_0110575003_p548514121007"></a><a name="zh-cn_topic_0110575003_p548514121007"></a>关联该IP地址对象的代理，用户也可以不设置，关联所有代理。</p>
    <p id="zh-cn_topic_0110575003_p248611216019"><a name="zh-cn_topic_0110575003_p248611216019"></a><a name="zh-cn_topic_0110575003_p248611216019"></a>选择了代理之后，该对象只会在配置相应代理的策略规则时可选。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row97013138366"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p12701201303619"><a name="zh-cn_topic_0110575003_p12701201303619"></a><a name="zh-cn_topic_0110575003_p12701201303619"></a>数据库</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p1247819131018"><a name="zh-cn_topic_0110575003_p1247819131018"></a><a name="zh-cn_topic_0110575003_p1247819131018"></a>关联该IP地址对象的数据库，用户也可以不设置，关联所有数据库。</p>
    <p id="zh-cn_topic_0110575003_p947820136015"><a name="zh-cn_topic_0110575003_p947820136015"></a><a name="zh-cn_topic_0110575003_p947820136015"></a>选择了数据库之后，该对象只会在配置相应数据库的策略规则时可选。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row1701141310363"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p770201343615"><a name="zh-cn_topic_0110575003_p770201343615"></a><a name="zh-cn_topic_0110575003_p770201343615"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p1770261313366"><a name="zh-cn_topic_0110575003_p1770261313366"></a><a name="zh-cn_topic_0110575003_p1770261313366"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p146721851135511"><a name="zh-cn_topic_0110575003_p146721851135511"></a><a name="zh-cn_topic_0110575003_p146721851135511"></a>输入IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row8598193353819"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p1959933313816"><a name="zh-cn_topic_0110575003_p1959933313816"></a><a name="zh-cn_topic_0110575003_p1959933313816"></a>子网掩码</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p11672551195510"><a name="zh-cn_topic_0110575003_p11672551195510"></a><a name="zh-cn_topic_0110575003_p11672551195510"></a>使用下拉框设置子网掩码。</p>
    <p id="zh-cn_topic_0110575003_p1241219397816"><a name="zh-cn_topic_0110575003_p1241219397816"></a><a name="zh-cn_topic_0110575003_p1241219397816"></a>子网掩码默认值为<span class="parmvalue" id="zh-cn_topic_0110575003_parmvalue63213503453"><a name="zh-cn_topic_0110575003_parmvalue63213503453"></a><a name="zh-cn_topic_0110575003_parmvalue63213503453"></a>“255.255.255.255”</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row1780193323818"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p578093353815"><a name="zh-cn_topic_0110575003_p578093353815"></a><a name="zh-cn_topic_0110575003_p578093353815"></a>IP范围</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p7780123310385"><a name="zh-cn_topic_0110575003_p7780123310385"></a><a name="zh-cn_topic_0110575003_p7780123310385"></a>起始IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p141176411434"><a name="zh-cn_topic_0110575003_p141176411434"></a><a name="zh-cn_topic_0110575003_p141176411434"></a>输入IP范围的起始IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row1995017330389"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p11951033173816"><a name="zh-cn_topic_0110575003_p11951033173816"></a><a name="zh-cn_topic_0110575003_p11951033173816"></a>结束IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p171190414436"><a name="zh-cn_topic_0110575003_p171190414436"></a><a name="zh-cn_topic_0110575003_p171190414436"></a>输入IP范围的结束IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row1098761718117"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p118352411112"><a name="zh-cn_topic_0110575003_p118352411112"></a><a name="zh-cn_topic_0110575003_p118352411112"></a>IP地址组</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p410682019115"><a name="zh-cn_topic_0110575003_p410682019115"></a><a name="zh-cn_topic_0110575003_p410682019115"></a>可用成员</p>
    </td>
    <td class="cellrowborder" valign="top" width="65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0110575003_p189231851141115"><a name="zh-cn_topic_0110575003_p189231851141115"></a><a name="zh-cn_topic_0110575003_p189231851141115"></a>根据数据库类型、代理、数据库筛选的条件，显示可以添加到对象组的对象名称。</p>
    <p id="zh-cn_topic_0110575003_p5106112051113"><a name="zh-cn_topic_0110575003_p5106112051113"></a><a name="zh-cn_topic_0110575003_p5106112051113"></a>在<span class="parmname" id="zh-cn_topic_0110575003_parmname7811189294"><a name="zh-cn_topic_0110575003_parmname7811189294"></a><a name="zh-cn_topic_0110575003_parmname7811189294"></a>“可用成员”</span>列表中，双击要包含在组中的对象（或选中，然后单击<span class="uicontrol" id="zh-cn_topic_0110575003_uicontrol103058315295"><a name="zh-cn_topic_0110575003_uicontrol103058315295"></a><a name="zh-cn_topic_0110575003_uicontrol103058315295"></a>“添加”</span>），将其添加到<span class="parmname" id="zh-cn_topic_0110575003_parmname4170135162914"><a name="zh-cn_topic_0110575003_parmname4170135162914"></a><a name="zh-cn_topic_0110575003_parmname4170135162914"></a>“当前成员”</span>列表中。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575003_row445471831112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0110575003_p164691920151115"><a name="zh-cn_topic_0110575003_p164691920151115"></a><a name="zh-cn_topic_0110575003_p164691920151115"></a>当前成员</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0110575003_p167504141212"><a name="zh-cn_topic_0110575003_p167504141212"></a><a name="zh-cn_topic_0110575003_p167504141212"></a>显示已经添加到该对象组的对象名称。</p>
    <p id="zh-cn_topic_0110575003_p144690203116"><a name="zh-cn_topic_0110575003_p144690203116"></a><a name="zh-cn_topic_0110575003_p144690203116"></a>在<span class="parmname" id="zh-cn_topic_0110575003_parmname3612171962914"><a name="zh-cn_topic_0110575003_parmname3612171962914"></a><a name="zh-cn_topic_0110575003_parmname3612171962914"></a>“当前成员”</span>列表中，双击要移除的对象（或选中，然后单击<span class="uicontrol" id="zh-cn_topic_0110575003_uicontrol14349172662914"><a name="zh-cn_topic_0110575003_uicontrol14349172662914"></a><a name="zh-cn_topic_0110575003_uicontrol14349172662914"></a>“移除”</span>），将其从<span class="parmname" id="zh-cn_topic_0110575003_parmname5333111513296"><a name="zh-cn_topic_0110575003_parmname5333111513296"></a><a name="zh-cn_topic_0110575003_parmname5333111513296"></a>“当前成员”</span>列表中删除。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“创建“或“更新“。

