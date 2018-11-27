# 出方向SSL安全加密设置<a name="ZH-CN_TOPIC_0111166366"></a>

该任务指导用户设置出方向SSL安全加密。为HexaTier与不同数据库类型的通信设置协议版本、加密算法的密码级套件以及阻止未加密的连接。

## 操作步骤<a name="zh-cn_topic_0110575028_s94b0e69af68347efb25f894c8f533962"></a>

1.  在HexaTier主菜单上，单击“系统“。
2.  在导航树上，选择“SSL \> 出方向 \> 安全等级“。
3.  在“组件类型”所需的加密级别中，单击![](figures/编辑.png)。

    显示组件类型SSL安全等级页面。

4.  在工作区中，根据需要设置下列参数，然后单击“更新“。

    <a name="zh-cn_topic_0110575028_tf920ce01dbb34713afd73421ea407f18"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0110575028_r1ddcc0d1d4314eb6ac63c33de655c59f"><th class="cellrowborder" valign="top" width="23.87%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0110575028_a2ef3a579f04a4e729c95f0976541e754"><a name="zh-cn_topic_0110575028_a2ef3a579f04a4e729c95f0976541e754"></a><a name="zh-cn_topic_0110575028_a2ef3a579f04a4e729c95f0976541e754"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="76.13%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0110575028_a50910fb64df84ec3a2cddbae7fe8ea77"><a name="zh-cn_topic_0110575028_a50910fb64df84ec3a2cddbae7fe8ea77"></a><a name="zh-cn_topic_0110575028_a50910fb64df84ec3a2cddbae7fe8ea77"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0110575028_rcb9f36e9d3c343488d51da8e776ab6fa"><td class="cellrowborder" valign="top" width="23.87%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0110575028_a7c13d542632e460b818dcd7bf871db82"><a name="zh-cn_topic_0110575028_a7c13d542632e460b818dcd7bf871db82"></a><a name="zh-cn_topic_0110575028_a7c13d542632e460b818dcd7bf871db82"></a>协议版本</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.13%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0110575028_a315110b2742a4219a5bba583251870ef"><a name="zh-cn_topic_0110575028_a315110b2742a4219a5bba583251870ef"></a><a name="zh-cn_topic_0110575028_a315110b2742a4219a5bba583251870ef"></a>要求的最低协议，包括：</p>
    <a name="zh-cn_topic_0110575028_u155a0099b1b94b72bbbd4d1d89bf2212"></a><a name="zh-cn_topic_0110575028_u155a0099b1b94b72bbbd4d1d89bf2212"></a><ul id="zh-cn_topic_0110575028_u155a0099b1b94b72bbbd4d1d89bf2212"><li>TLS 1.2</li><li>TLS 1.1</li><li>TLS 1.0</li><li>SSL 3.0</li><li>SSL 2.0</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575028_rc05e7629da764ed4949b538519c3ccef"><td class="cellrowborder" valign="top" width="23.87%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0110575028_a555e172cad954413957ddecef948db32"><a name="zh-cn_topic_0110575028_a555e172cad954413957ddecef948db32"></a><a name="zh-cn_topic_0110575028_a555e172cad954413957ddecef948db32"></a>密码级别</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.13%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0110575028_a992ab418039e4a79a638ddc46d6e2d0a"><a name="zh-cn_topic_0110575028_a992ab418039e4a79a638ddc46d6e2d0a"></a><a name="zh-cn_topic_0110575028_a992ab418039e4a79a638ddc46d6e2d0a"></a>要求的最低加密算法套件。密码级别包括：</p>
    <a name="zh-cn_topic_0110575028_uc697bc29772e430d92e90e9cf016b462"></a><a name="zh-cn_topic_0110575028_uc697bc29772e430d92e90e9cf016b462"></a><ul id="zh-cn_topic_0110575028_uc697bc29772e430d92e90e9cf016b462"><li>高：最高级别的安全，非向后兼容。</li><li>中：中级安全和部分向后兼容。</li><li>向后兼容：最低级别的安全和向后兼容。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0110575028_r47a98d6cbc434669916f7c64a315f240"><td class="cellrowborder" valign="top" width="23.87%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0110575028_aa2e10623225848df898a1ff570dcf0e9"><a name="zh-cn_topic_0110575028_aa2e10623225848df898a1ff570dcf0e9"></a><a name="zh-cn_topic_0110575028_aa2e10623225848df898a1ff570dcf0e9"></a>阻止未加密的连接</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.13%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0110575028_a2b88b83f0c8b4016ab983aea53c9f3d7"><a name="zh-cn_topic_0110575028_a2b88b83f0c8b4016ab983aea53c9f3d7"></a><a name="zh-cn_topic_0110575028_a2b88b83f0c8b4016ab983aea53c9f3d7"></a>通过勾选该参数，可以要求新的受保护数据库使用SSL。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   TLS 1.0只是为了兼容MySQL，存在安全隐患，请谨慎使用。  
    >-   由于DDM不支持SSL连接，因此，HexaTier与DDM之间的连接为非加密连接。  


## 删除SSL安全例外<a name="zh-cn_topic_0110575028_section78421747134214"></a>

1.  在HexaTier主菜单上，单击“系统“。
2.  在导航树上，选择“SSL \> 出方向 \> 安全等级“。
3.  在例外列表中，找到所需的例外，单击![](figures/删除.png)删除例外。

