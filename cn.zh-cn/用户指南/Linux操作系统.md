# Linux操作系统<a name="ZH-CN_TOPIC_0174227115"></a>

Agent添加完成后，您还需要下载Agent，并根据Agent的添加方式在数据库端或应用端安装Agent，将添加的数据库连接到数据库安全审计实例，才能使用数据库安全审计功能。

## 前提条件<a name="section070891116319"></a>

-   已成功购买数据库安全审计实例，且实例的状态为“运行中“。
-   数据库已成功添加Agent。
-   已获取Linux操作系统Agent安装包。
-   安装Agent节点的运行系统满足Linux系统版本要求。有关Linux系统版本的要求，请参见[Agent可以安装在哪些Linux操作系统上？](https://support.huaweicloud.com/dbss_faq/dbss_01_0319.html)。

## 安装Agent<a name="section16540958125719"></a>

请根据您在云上实际部署的数据库，将Agent安装在数据库端、应用端或代理端。

有关Agent安装节点的详细说明，请参见[如何选择数据库安全审计的Agent安装节点？](https://support.huaweicloud.com/dbss_faq/dbss_01_0282.html)。

-   ECS/BMS的自建数据库

    在数据库端、应用端或代理端安装Agent

-   RDS关系型数据库

    在应用端或代理端安装Agent


1.  将下载的Agent安装包“xxx.tar“上传到待安装Agent的节点（例如使用WinSCP工具）。
2.  使用跨平台远程访问工具（例如PuTTY）以**root**用户通过SSH方式，登录该节点。
3.  执行以下命令，进入Agent安装包“xxx.tar“所在目录。

    **cd** _Agent安装包所在目录_

4.  执行以下命令，解压缩“xxx.tar“安装包。

    **tar** **-xvf** _xxx.tar_

5.  执行以下命令，进入解压后的目录。

    **cd** _解压后的目录_

6.  执行以下命令，查看是否有安装脚本“install.sh“的执行权限。

    **ll**

    -   如果有安装脚本的执行权限，请执行[7](#li144058161155)。
    -   如果没有安装脚本的执行权限，请执行以下操作：
        1.  执行以下命令，添加安装脚本执行权限。

            **chmod +x install.sh**

        2.  确认有安装脚本执行权限后，请执行[7](#li144058161155)。

7.  <a name="li144058161155"></a>执行以下命令，安装Agent。

    **sh** **install.sh**

    如果界面回显以下信息，说明安装成功。否则，说明Agent安装失败。

    ```
    start agent
    starting audit agent
    audit agent started
    start success
    install dbss audit agent done!
    ```

    >![](public_sys-resources/icon-notice.gif) **须知：**   
    >如果Agent安装失败，请您确认安装节点的运行系统是否满足Linux操作系统要求，并重新安装Agent。  

8.  执行以下命令，查看Agent程序的运行状态。

    **service** **audit\_agent status**

    如果界面回显以下信息，说明Agent程序运行正常。

    ```
    audit agent is running.
    ```


## 效果验证<a name="section159134316157"></a>

1.  <a name="li0294761612"></a>Agent安装成功后，在数据库上执行一条SQL语句（例如“select \* from mysql.user limit 1“）。
2.  [登录管理控制台](https://console.huaweicloud.com/)。
3.  验证Agent与数据库安全审计实例的网络通信正常。
    1.  进入SQL语句列表入口，如[图1](#fig1489915095118)所示。

        **图 1**  进入SQL语句列表入口<a name="fig1489915095118"></a>  
        ![](figures/进入SQL语句列表入口.png "进入SQL语句列表入口")

    2.  在“时间“所在行右侧，单击![](figures/日历.png)，选择开始时间和结束时间，单击“提交“，SQL语句列表将显示[1](#li0294761612)中输入的SQL语句，如[图2](#fig8994029155516)所示。

        **图 2**  查看SQL语句<a name="fig8994029155516"></a>  
        ![](figures/查看SQL语句.png "查看SQL语句")

        -   如果SQL语句列表中显示输入的SQL语句，说明Agent与数据库安全审计实例之间网络通信正常。
        -   如果SQL语句列表中未显示输入的SQL语句，说明Agent与数据库安全审计实例之间网络通信异常，请参照[Agent与数据库安全审计实例之间通信异常](Agent与数据库安全审计实例之间通信异常.md)处理。



## 后续处理<a name="section11581123681920"></a>

数据库安全审计默认提供一条“全审计规则“的审计范围，可以对成功连接数据库安全审计实例的所有数据库进行安全审计。Agent安装完成后，您可以查看被添加的数据库的审计结果。详细操作，请参见[查看审计结果](查看审计总览信息.md)。

## 相关操作<a name="section3657198173220"></a>

-   有关添加Agent的详细操作，请参见[步骤二：添加Agent](步骤二-添加Agent.md)。
-   数据库开启SSL时，将不能使用数据库安全审计功能。如果您需要使用数据库安全审计功能，请关闭数据库的SSL。关闭数据库SSL的详细操作，请参见[如何关闭数据库SSL？](https://support.huaweicloud.com/dbss_faq/dbss_01_0283.html)。
-   有关卸载Agent的详细操作，请参见[卸载Agent](卸载Agent.md)。

