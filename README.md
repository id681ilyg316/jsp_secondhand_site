## 本项目实现的最终作用是基于JSP校园二手物品交易平台网站
## 分为3个角色
### 第1个角色为管理员角色，实现了如下功能：
 - 二手交易管理
 - 优惠活动管理
 - 友情链接管理
 - 物品分类管理
 - 用户管理
 - 留言板管理
 - 管理员登录
 - 网站公告管理
 - 订单管理
### 第2个角色为设计文稿，实现了如下功能：
 - 论文截图
### 第3个角色为用户角色，实现了如下功能：
 - 个人订单管理
 - 二手交易查看
 - 优惠新闻查看
 - 提交订单
 - 查看网站介绍和信息
 - 查看购物车
 - 用户注册和登录
 - 用户角色登录
 - 留言板管理
 - 购买商品
## 数据库设计如下：
# 数据库设计文档

**数据库名：** secondhand_site

**文档版本：** 


| 表名                  | 说明       |
| :---: | :---: |
| [fwly](#fwly) |  |
| [fwpl](#fwpl) |  |
| [hbnews](#hbnews) |  |
| [messages](#messages) |  |
| [proscar](#proscar) |  |
| [prosorders](#prosorders) |  |
| [scj](#scj) |  |
| [secondhand](#secondhand) |  |
| [users](#users) |  |
| [wpfl](#wpfl) |  |
| [yqlj](#yqlj) |  |
| [zdatadic](#zdatadic) |  |

**表名：** <a id="fwly">fwly</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | title |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 标题  |
|  3   | saver |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  4   | content |   text   | 65535 |   0    |    Y     |  N   |   NULL    | 内容  |
|  5   | savetime |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 保存时间  |

**表名：** <a id="fwpl">fwpl</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | fwid |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  3   | saver |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  4   | saverimg |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  5   | content |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 内容  |
|  6   | savetime |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 保存时间  |

**表名：** <a id="hbnews">hbnews</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | title |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 标题  |
|  3   | author |   varchar   | 64 |   0    |    Y     |  N   |   NULL    | 作者  |
|  4   | filename |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 文件名  |
|  5   | content |   varchar   | 1024 |   0    |    Y     |  N   |   NULL    | 内容  |
|  6   | savetime |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 保存时间  |

**表名：** <a id="messages">messages</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | saver |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  3   | savetime |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  4   | content |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 内容  |
|  5   | resaver |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  6   | recontent |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  7   | resavetime |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="proscar">proscar</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | uname |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  3   | touname |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  4   | pname |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  5   | price |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 价格  |
|  6   | filename |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 文件名  |
|  7   | status |   varchar   | 64 |   0    |    Y     |  N   |   NULL    | 状态  |
|  8   | savetime |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  9   | nums |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="prosorders">prosorders</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | uname |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  3   | touname |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  4   | ddinfo |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  5   | lxr |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 联系人  |
|  6   | lxtel |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  7   | lxqq |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  8   | addrs |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  9   | fkfs |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  10   | status |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 状态  |
|  11   | savetime |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="scj">scj</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | sctype |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  3   | uname |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 用户名  |
|  4   | wid |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="secondhand">secondhand</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | title |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 标题  |
|  3   | wpbei |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  4   | filename |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 文件名  |
|  5   | lxr |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 联系人  |
|  6   | lxtel |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  7   | lxaddrs |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  8   | lxqq |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  9   | price |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 价格  |
|  10   | uname |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  11   | savetime |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  12   | infotype |   varchar   | 64 |   0    |    Y     |  N   |   NULL    | 信息类型  |
|  13   | wptype |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="users">users</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | username |   varchar   | 64 |   0    |    Y     |  N   |   NULL    | 用户名  |
|  3   | userpass |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  4   | truename |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  5   | sex |   varchar   | 8 |   0    |    Y     |  N   |   NULL    | 性别  |
|  6   | qq |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  7   | phoneno |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  8   | email |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 邮箱  |
|  9   | dizhi |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  10   | usertype |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 用户类型  |
|  11   | filename |   varchar   | 64 |   0    |    Y     |  N   |   NULL    | 文件名  |
|  12   | savetime |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="wpfl">wpfl</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | typename |   varchar   | 64 |   0    |    Y     |  N   |   NULL    | 类型名称  |

**表名：** <a id="yqlj">yqlj</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | ljname |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  3   | ljurl |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="zdatadic">zdatadic</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | datatype |   varchar   | 64 |   0    |    Y     |  N   |   NULL    |   |
|  3   | content |   text   | 65535 |   0    |    Y     |  N   |   NULL    | 内容  |

**运行不出来可以微信 javape 我的公众号：源码码头**
