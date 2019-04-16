# 卸载Agent<a name="ZH-CN_TOPIC_0146117470"></a>

在数据库端或应用端安装Agent后，当不需要审计数据库时，您可以在该数据库的数据库端或应用端卸载Agent。

## 前提条件<a name="section070891116319"></a>

-   已在数据库端或应用端停止Agent程序。
-   已成功关闭数据库端或应用端所在数据库安全审计。

## 卸载Agent<a name="section7772833173515"></a>

1.  使用跨平台远程访问工具（例如PuTTY）以**root**用户通过SSH方式，登录数据库端或应用端。
2.  执行以下命令，进入“Agent.tar“安装包解压后所在目录。

    **cd** _Agent安装包解压后所在目录_

3.  执行以下命令，卸载Agent。

    **sh** **uninstall.sh**

    如果界面回显以下信息，说明卸载成功。

    ```
    uninstall audit agent...
    exist os-release file
    stopping audit agent
    audit agent stopped
    stop audit_agent success
    service audit_agent does not support chkconfig
    uninstall audit agent completed!
    ```


