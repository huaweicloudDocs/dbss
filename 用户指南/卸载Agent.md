# 卸载Agent<a name="dbss_01_0199"></a>

在数据库端或应用端的节点安装Agent后，当不需要停止审计数据库时，您可以在安装Agent的节点卸载Agent。

## 前提条件<a name="section070891116319"></a>

已在安装节点安装了Agent程序。

## 在Linux操作系统上卸载Agent<a name="section7772833173515"></a>

1.  使用跨平台远程访问工具（例如PuTTY）以**root**用户通过SSH方式，登录已安装Agent的节点。
2.  执行以下命令，进入Agent安装包“xxx.tar.gz“解压后所在目录。

    **cd** _Agent安装包解压后所在目录_

3.  执行以下命令，查看是否有卸载脚本“uninstall.sh“的执行权限。

    **ll**

    -   如果有卸载脚本的执行权限，请执行[4](#li144058161155)。
    -   如果没有卸载脚本的执行权限，请执行以下操作：
        1.  执行以下命令，添加卸载脚本执行权限。

            **chmod +x uninstall.sh**

        2.  确认有安装脚本执行权限后，请执行[4](#li144058161155)。

4.  <a name="li144058161155"></a>执行以下命令，卸载Agent。

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


## 在Windows操作系统上卸载Agent<a name="section11227183015414"></a>

1.  进入Agent安装文件的目录。
2.  双击“uninstall.bat“执行文件，卸载Agent。
3.  验证Agent已卸载成功。
    1.  打开任务管理器，查看“dbss\_audit\_agent“进程已停止。
    2.  查看Agent安装目录，安装目录内容已经全部删除。


