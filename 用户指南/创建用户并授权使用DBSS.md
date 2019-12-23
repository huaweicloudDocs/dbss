# 创建用户并授权使用DBSS<a name="ZH-CN_TOPIC_0169801941"></a>

通过简单的用户组授权方法，将DBSS服务的策略授予用户组，并将用户添加至用户组中，从而使用户拥有对应的DBSS权限。

操作流程如[图1](#fig4754165816356)所示。

## 示例流程<a name="section1679719365337"></a>

**图 1**  给用户授权服务权限流程<a name="fig4754165816356"></a>  
![](figures/给用户授权服务权限流程.png "给用户授权服务权限流程")

1.  <a name="li8135822590"></a>创建用户组并授权。

    在IAM控制台创建用户组，并授予数据库安全服务的管理员权限“DBSS Security Administrator“。

2.  创建用户。

    在IAM控制台创建用户，并将其加入[1](#li8135822590)中创建的用户组。

3.  用户登录并验证权限。

    新创建的用户登录控制台，验证数据库安全服务的管理员权限。


## 前提条件<a name="section350215143713"></a>

给用户组授权之前，请您了解用户组可以添加的DBSS系统策略，并结合实际需求进行选择，DBSS系统策略如[表1](#table198221859141416)所示。若您需要对除DBSS之外的其它服务授权，IAM支持服务的所有策略请参见[权限策略](https://support.huaweicloud.com/usermanual-permissions/zh-cn_topic_0063498930.html)。

**表 1**  DBSS系统策略

<a name="table198221859141416"></a>
<table><thead align="left"><tr id="zh-cn_topic_0169801624_row84517413132"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0169801624_p94513416133"><a name="zh-cn_topic_0169801624_p94513416133"></a><a name="zh-cn_topic_0169801624_p94513416133"></a>策略名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0169801624_p5451194161319"><a name="zh-cn_topic_0169801624_p5451194161319"></a><a name="zh-cn_topic_0169801624_p5451194161319"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0169801624_p104511346139"><a name="zh-cn_topic_0169801624_p104511346139"></a><a name="zh-cn_topic_0169801624_p104511346139"></a>依赖关系</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0169801624_row945120416134"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0169801624_p18451448135"><a name="zh-cn_topic_0169801624_p18451448135"></a><a name="zh-cn_topic_0169801624_p18451448135"></a>DBSS System Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0169801624_ul1494151155714"></a><a name="zh-cn_topic_0169801624_ul1494151155714"></a><ul id="zh-cn_topic_0169801624_ul1494151155714"><li>数据库安全防护操作权限：<a name="zh-cn_topic_0169801624_ul13762320391"></a><a name="zh-cn_topic_0169801624_ul13762320391"></a><ul id="zh-cn_topic_0169801624_ul13762320391"><li>购买实例。</li><li>获取实例列表。</li><li>开启、关闭、重启实例。</li><li>升级服务实例。</li><li>绑定、解绑弹性IP。</li><li>登录数据库安全管理控制台。</li></ul>
</li><li>数据库安全审计操作权限：<a name="zh-cn_topic_0169801624_ul19400133010115"></a><a name="zh-cn_topic_0169801624_ul19400133010115"></a><ul id="zh-cn_topic_0169801624_ul19400133010115"><li>购买实例。</li><li>开启、关闭、重启实例。</li><li>获取实例列表。</li><li>获取基本信息。</li><li>获取审计概况。</li><li>获取监控信息。</li><li>获取操作日志。</li><li>数据库管理。</li><li>Agent管理。</li><li>邮件设置。</li><li>备份与恢复。</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><div class="p" id="zh-cn_topic_0169801624_p345244171320"><a name="zh-cn_topic_0169801624_p345244171320"></a><a name="zh-cn_topic_0169801624_p345244171320"></a>购买实例需要同时具有VPC Admin和BSS Administrator策略。<a name="zh-cn_topic_0169801624_ul060520367114"></a><a name="zh-cn_topic_0169801624_ul060520367114"></a><ul id="zh-cn_topic_0169801624_ul060520367114"><li>VPC Admin：对虚拟私有云的所有执行权限。项目级策略，在同项目中勾选。</li><li>BSS Administrator：对账号中心、费用中心、资源中心中的所有菜单项执行任意操作。项目级策略，在同项目中勾选。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0169801624_row14833241193015"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0169801624_p11835124183018"><a name="zh-cn_topic_0169801624_p11835124183018"></a><a name="zh-cn_topic_0169801624_p11835124183018"></a>DBSS Audit Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0169801624_ul1318011278580"></a><a name="zh-cn_topic_0169801624_ul1318011278580"></a><ul id="zh-cn_topic_0169801624_ul1318011278580"><li>数据库安全防护操作权限：<a name="zh-cn_topic_0169801624_ul77271516171210"></a><a name="zh-cn_topic_0169801624_ul77271516171210"></a><ul id="zh-cn_topic_0169801624_ul77271516171210"><li>获取实例列表。</li><li>登录数据库安全服务管理控制台。</li></ul>
</li></ul>
<a name="zh-cn_topic_0169801624_ul19876172691219"></a><a name="zh-cn_topic_0169801624_ul19876172691219"></a><ul id="zh-cn_topic_0169801624_ul19876172691219"><li>数据库安全审计操作权限：<a name="zh-cn_topic_0169801624_ul16566459171311"></a><a name="zh-cn_topic_0169801624_ul16566459171311"></a><ul id="zh-cn_topic_0169801624_ul16566459171311"><li>获取实例列表。</li><li>获取基本信息。</li><li>获取审计概况。</li><li>获取报表结果。</li><li>获取规则信息。</li><li>获取语句信息。</li><li>获取会话信息。</li><li>获取监控信息。</li><li>获取操作日志。</li><li>获取数据库列表。</li><li>报表管理。</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0169801624_p168351741103014"><a name="zh-cn_topic_0169801624_p168351741103014"></a><a name="zh-cn_topic_0169801624_p168351741103014"></a>无</p>
</td>
</tr>
<tr id="zh-cn_topic_0169801624_row1431194710395"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0169801624_p631244773912"><a name="zh-cn_topic_0169801624_p631244773912"></a><a name="zh-cn_topic_0169801624_p631244773912"></a>DBSS Security Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0169801624_ul4237657291748"></a><a name="zh-cn_topic_0169801624_ul4237657291748"></a><ul id="zh-cn_topic_0169801624_ul4237657291748"><li>数据库安全防护操作权限：<a name="zh-cn_topic_0169801624_ul66261930165"></a><a name="zh-cn_topic_0169801624_ul66261930165"></a><ul id="zh-cn_topic_0169801624_ul66261930165"><li>获取实例列表。</li><li>登录数据库安全服务管理控制台。</li></ul>
</li><li>数据库安全审计操作权限：<a name="zh-cn_topic_0169801624_ul4158741191517"></a><a name="zh-cn_topic_0169801624_ul4158741191517"></a><ul id="zh-cn_topic_0169801624_ul4158741191517"><li>获取实例列表。</li><li>获取基本信息。</li><li>获取审计概况。</li><li>获取报表结果。</li><li>获取规则信息。</li><li>获取语句信息。</li><li>获取会话信息。</li><li>获取监控信息。</li><li>获取操作日志。</li><li>获取数据库列表。</li><li>审计规则设置。</li><li>告警通知设置。</li><li>报表管理。</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0169801624_p20313147193914"><a name="zh-cn_topic_0169801624_p20313147193914"></a><a name="zh-cn_topic_0169801624_p20313147193914"></a>无</p>
</td>
</tr>
</tbody>
</table>

## 步骤1：创建用户组并授权<a name="section47421555114919"></a>

用户组是用户的集合，IAM通过用户组功能实现用户的授权。您在IAM中创建的用户，需要加入特定用户组后，用户才具备用户组所拥有的权限。关于创建用户组并给用户组授权的方法，可以参考如下操作。

1.  使用注册的华为云账号登录华为云，登录时请选择“账号登录“。

    **图 2**  账号登录<a name="zh-cn_topic_0169425415_zh-cn_topic_0154973652_fig184406496424"></a>  
    ![](figures/账号登录-0.png "账号登录-0")

2.  进入华为云控制台，控制台页面中单击右上角的用户名，选择“统一身份认证“。

    **图 3**  服务选择<a name="zh-cn_topic_0169425415_fig192441010165114"></a>  
    ![](figures/服务选择.png "服务选择")

3.  在统一身份认证服务的左侧导航空格中，单击“用户组  \>  创建用户组“。

    **图 4**  创建用户组<a name="zh-cn_topic_0169425415_fig135481549125111"></a>  
    ![](figures/创建用户组.png "创建用户组")

4.  在“创建用户组“界面，输入“用户组名称“，以“data“为例，单击“确定“。

    用户组创建完成，界面自动返回用户组列表，列表中显示新建的用户组。

5.  单击新建用户组“data“右侧的“权限配置“。

    **图 5**  权限配置<a name="zh-cn_topic_0169425415_fig918317195211"></a>  
    ![](figures/权限配置.png "权限配置")

6.  在“用户组权限“页签中，单击列表左上方的“配置权限“。

    **图 6**  配置权限<a name="zh-cn_topic_0169425415_fig124391145132312"></a>  
    ![](figures/配置权限.png "配置权限")

7.  IAM提供“策略视图“和“项目视图“两种权限配置方式，两种方式产生的授权效果相同，请根据您的需求选择合适的方式。

    DBSS为项目级服务，请确认用户需要使用DBSS资源的项目，在对应项目中设置权限。设置完成后用户仅能访问授权项目中的DBSS资源，无法访问其他项目中的DBSS资源。

    -   策略视图：您可以为一个策略同时配置多个项目。
        1.  在右侧滑窗中，选中“策略视图“；在搜索框中搜索“DBSS“，以选择“DBSS System Administrator“为例；在“项目\[作用范围\]“下拉框中，选择需要给该策略授权的项目（可选择多个项目）。

            DBSS的系统策略说明，请参见：[DBSS系统策略](https://support.huaweicloud.com/productdesc-dbss/dbss_01_0241.html)。

            **图 7**  选择策略和项目<a name="fig15856182122911"></a>  
            ![](figures/选择策略和项目.png "选择策略和项目")

        2.  单击“确定“，完成该用户组授权。

    -   项目视图：您可以为一个项目同时配置多个策略。
        1.  在右侧滑窗中，单击“项目视图“；选择需要授权的“项目\[作用范围\]“，单击右侧的“选择策略“。

            **图 8**  选择项目视图<a name="zh-cn_topic_0169425415_fig174066518293"></a>  
            ![](figures/选择项目视图.png "选择项目视图")

        2.  在“选择策略“弹窗中，搜索“DBSS“，以选择“DBSS System Administrator“为例。

            DBSS的系统策略说明，请参见：[DBSS系统策略](https://support.huaweicloud.com/productdesc-dbss/dbss_01_0241.html)。

            **图 9**  选择策略<a name="fig55971385018"></a>  
            ![](figures/选择策略.png "选择策略")

        3.  单击“确定“，完成用户组授权。



## 步骤2：创建IAM用户<a name="section1364975213584"></a>

IAM用户与企业中的实际员工或是应用程序相对应，有唯一的安全凭证，可以通过加入一个或多个用户组来获得用户组的权限。关于IAM用户的创建方式请参见如下步骤。

1.  在统一身份认证服务，左侧导航中，单击“用户  \>  创建用户“。
2.  在“创建用户“界面中填写“用户信息“。如需一次创建多个用户，可以单击“添加用户“进行批量创建，每次最多可创建10个用户。

    **图 10**  用户信息<a name="zh-cn_topic_0169425415_fig233618408535"></a>  
    ![](figures/用户信息.png "用户信息")

    -   用户名：用户登录华为云的用户名，以“James“为例。
    -   邮箱：IAM用户绑定的邮箱，仅“访问方式“选择“首次登录时设置“时必填，选择其他访问方式时选填。
    -   手机号（选填）：IAM用户绑定的手机号。
    -   描述（可选）：对用户的描述信息。

3.  在“创建用户“页面选择“访问方式“，完成后单击“下一步“。

    **图 11**  访问方式<a name="zh-cn_topic_0169425415_fig558915354115"></a>  
    ![](figures/访问方式.png "访问方式")

    -   编程访问：创建用户完成后即可下载本次创建的所有用户的[访问密钥](https://support.huaweicloud.com/usermanual-ca/zh-cn_topic_0046606340.html)。
    -   华为云管理控制台访问：用户可以使用账号密码登录到华为云管理控制台。
        -   控制台登录密码设置方式：当一次创建多个用户时，密码设置方式可选择“首次登录时设置“和“自定义“，不支持“自动生成“密码；当仅创建一个用户时，以上方式均可选择。
        -   登录保护：为了您的账号安全，建议选择“开启登录保护“。后续如需开启或关闭登录保护，请参见：[登录保护](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0079477316.html)。

4.  （可选）将用户加入到用户组，完成后单击“下一步“。
    -   选择新创建的用户组“data“。将用户加入用户组，用户将具备用户组的权限，这一过程即给该用户授权。其中“admin“为系统缺省提供的用户组，具有管理人员以及所有云服务资源的操作权限。
    -   如需创建新的用户组，可单击“创建用户组“，填写用户组名称和描述（可选），创建成功后即可将用户加入到新创建的用户组中。

5.  IAM用户创建成功，用户列表中显示新创建的IAM用户。如果在访问方式中勾选了“编程访问“，可在此页面下载访问密钥，后续也可以在“我的凭证“中[管理访问密钥](https://support.huaweicloud.com/usermanual-ca/zh-cn_topic_0046606340.html)。

    **图 12**  创建成功<a name="zh-cn_topic_0169425415_fig12238144920189"></a>  
    ![](figures/创建成功.png "创建成功")


## 步骤3：用户登录并验证权限<a name="section510119383012"></a>

用户创建完成后，可以使用新用户的用户名及身份凭证登录华为云验证权限，即“DBSS System Administrator“权限。更多用户登录方法请参见[用户登录华为云方法](https://support.huaweicloud.com/qs-iam/iam_01_0031.html)。

1.  在华为云登录页面，单击右下角的“IAM用户登录“。

    **图 13**  IAM用户登录<a name="zh-cn_topic_0169425415_fig8273258155316"></a>  
    ![](figures/IAM用户登录-1.png "IAM用户登录-1")

2.  在“IAM用户登录“页面，输入账号名、用户名及用户密码，使用新创建的用户登录。

    -   账号名为该IAM用户所属华为云账号的名称。
    -   用户名和密码为账号在IAM创建用户时输入的用户名和密码。

    如果登录失败，您可以联系您的账号主体，确认用户名及密码是否正确，或是重置用户名及密码，重置方法请参见：[忘记IAM用户密码](https://support.huaweicloud.com/iam_faq/iam_01_0314.html#section1)。

3.  登录成功后，进入华为云控制台，登录后默认区域为“华北-北京一“。
4.  在“服务列表“中选择除数据库安全服务外的任一服务，若提示权限不足，表示“DBSS System Administrator“已生效。

