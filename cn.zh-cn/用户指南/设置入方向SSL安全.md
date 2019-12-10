# 设置入方向SSL安全<a name="ZH-CN_TOPIC_0111166358"></a>

该任务指导用户设置入方向SSL安全，来保护客户端和HexaTier之间的通信。用户可以设置最低协议版本、加密算法的密码级套件以及阻止客户端与HexaTier未加密的连接。

## 操作步骤<a name="zh-cn_topic_0180960226_s177dd9d067c4486783a3419f2348583f"></a>

1.  在HexaTier主菜单上，单击“系统“。
2.  在导航树上，选择“SSL \> 入方向 \> 安全等级“。
3.  在工作区中，根据需要设置参数，然后单击“更新“。

    **表 1**  SSL入方向安全参数

    <a name="zh-cn_topic_0180960226_t284bb296fc4b4619a2ed7e14d44cce84"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0180960226_rd90f436bd525408eb6f5c80a1db4cc85"><th class="cellrowborder" valign="top" width="25.369999999999997%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0180960226_a0cc0f5c1492d4084928f1c4f0c831d1e"><a name="zh-cn_topic_0180960226_a0cc0f5c1492d4084928f1c4f0c831d1e"></a><a name="zh-cn_topic_0180960226_a0cc0f5c1492d4084928f1c4f0c831d1e"></a>选项</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.63%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0180960226_aec9e02502a7d459ab546d3baa3009caa"><a name="zh-cn_topic_0180960226_aec9e02502a7d459ab546d3baa3009caa"></a><a name="zh-cn_topic_0180960226_aec9e02502a7d459ab546d3baa3009caa"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0180960226_r3064f2b26c034921b4a179da21a2ddec"><td class="cellrowborder" valign="top" width="25.369999999999997%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960226_a211dce73e288419f8f8939d5936924f1"><a name="zh-cn_topic_0180960226_a211dce73e288419f8f8939d5936924f1"></a><a name="zh-cn_topic_0180960226_a211dce73e288419f8f8939d5936924f1"></a>协议版本</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.63%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960226_a4bcdbee0ee114803a60200d605d746a0"><a name="zh-cn_topic_0180960226_a4bcdbee0ee114803a60200d605d746a0"></a><a name="zh-cn_topic_0180960226_a4bcdbee0ee114803a60200d605d746a0"></a>要求的最低协议，包括：</p>
    <a name="zh-cn_topic_0180960226_u14549cdfb97f4f2db9598bebcebff36b"></a><a name="zh-cn_topic_0180960226_u14549cdfb97f4f2db9598bebcebff36b"></a><ul id="zh-cn_topic_0180960226_u14549cdfb97f4f2db9598bebcebff36b"><li>TLS 1.2</li><li>TLS 1.1</li><li>TLS 1.0</li><li>SSL 3.0</li><li>SSL 2.0</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960226_ra9b917a38d874b4ab91301bec3e8c36d"><td class="cellrowborder" valign="top" width="25.369999999999997%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960226_a3798d9d9dd87443098be7b07047d3c81"><a name="zh-cn_topic_0180960226_a3798d9d9dd87443098be7b07047d3c81"></a><a name="zh-cn_topic_0180960226_a3798d9d9dd87443098be7b07047d3c81"></a>密码级别</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.63%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960226_abb2d373cbeda4d18b9abbe5ee1f44c0d"><a name="zh-cn_topic_0180960226_abb2d373cbeda4d18b9abbe5ee1f44c0d"></a><a name="zh-cn_topic_0180960226_abb2d373cbeda4d18b9abbe5ee1f44c0d"></a>要求的低加密算法套件。密码级别包括：</p>
    <a name="zh-cn_topic_0180960226_u5a81c4217c6446feb0c4b313a577c374"></a><a name="zh-cn_topic_0180960226_u5a81c4217c6446feb0c4b313a577c374"></a><ul id="zh-cn_topic_0180960226_u5a81c4217c6446feb0c4b313a577c374"><li>高：高级别的安全，非向后兼容。</li><li>中：中级安全和部分向后兼容。</li><li>向后兼容：低级别的安全和向后兼容。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0180960226_r3e29b77ed1684684810bd02dd6ab0e61"><td class="cellrowborder" valign="top" width="25.369999999999997%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0180960226_a36720f3fd8684eddaaa24c8854f7b23d"><a name="zh-cn_topic_0180960226_a36720f3fd8684eddaaa24c8854f7b23d"></a><a name="zh-cn_topic_0180960226_a36720f3fd8684eddaaa24c8854f7b23d"></a>阻止未加密的连接</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.63%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0180960226_add46f4ba01a8400c8bb949d564c8265f"><a name="zh-cn_topic_0180960226_add46f4ba01a8400c8bb949d564c8265f"></a><a name="zh-cn_topic_0180960226_add46f4ba01a8400c8bb949d564c8265f"></a>通过勾选该参数，可以要求新的受保护数据库使用SSL。</p>
    </td>
    </tr>
    </tbody>
    </table>


