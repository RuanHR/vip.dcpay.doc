# 基础Param

## PaginationParam
[PaginationParam]:#PaginationParam

> 分页查询基础参数

| 字段     | 类型 | 是否必传 | 说明                       |
| -------- | ---- | -------- | -------------------------- |
| pageNum  | int  | 是       | 当前页码.从1开始           |
| pageSize | int  | 是       | 当前页预期最大条数,最大100 |



# 基础VO

## GIIdentity

> 基础ID信息类型，泛型类型是id的类型

[GIIdentity]: #GIIdentity

| 字段    | 类型   | 说明   | 跳转 |
| ------- | ------ | ------ | ---- |
| id      | T      | id值   |      |
| account | string | 账户值 |      |

## Property

> 基础属性，泛型类型是code的类型

[Property]: #Property

| 字段 | 类型   | 说明               | 跳转 |
| ---- | ------ | ------------------ | ---- |
| code | T      | 属性的code码       |      |
| name | String | 属性的默认显示名称 |      |


## Currency

[Currency]: #Currency

> 币种信息，继承自 [Property][Property]<String>

| 字段      | 类型   | 说明           | 跳转 |
| --------- | ------ | -------------- | ---- |
| icon      | String | 币种的icon地址 |      |
| symbol    | String | 币种的符号     |      |
| precision | int    | 币种的精度     |      |


## TimePair

[TimePair]: #TimePair

> 时间对信息

| 字段   | 类型 | 说明     | 跳转 |
| ------ | ---- | -------- | ---- |
| create | date | 创建时间 |      |
| modify | date | 修改时间 |      |

## Pagination

[Pagination]: #Pagination

> 页码信息

| 字段  | 类型 | 说明           | 跳转 |
| ----- | ---- | -------------- | ---- |
| num   | int  | 当前页码       |      |
| size  | int  | 当前页最大条数 |      |
| total | int  | 总条数         |      |

## Page

[Page]:#Page

> 分页结构，泛型类型是content每条数据的类型

| 字段       | 类型     | 说明               | 跳转                     |
| ---------- | -------- | ------------------ | ------------------------ |
| pagination | object   | 分页页码信息       | [Pagination][Pagination] |
| content    | array<T> | 分页具体内容的数组 |                          |

# 资产业务VO

## AssetVo
[AssetVo]: #AssetVo

> 资产类型

| 字段     | 类型   | 说明                   | 跳转                 |
| -------- | ------ | ---------------------- | -------------------- |
| id       | long   | 资产id                 |                      |
| currency | object | 资产代表的币种         | [Currency][Currency] |
| free     | number | 可自由使用的钱\|热钱   |                      |
| unfree   | number | 不可自由使用的钱\|冷钱 |                      |
| time     | object | 资产信息时间对         | [TimePair][TimePair] |





# 配置业务VO

## GrabSwitch

[GrabSwitch]:#GrabSwitch

> 抢单开关配置

| 字段     | 类型 | 说明     | 跳转                                       |
| -------- | ---- | -------- | ------------------------------------------ |
| main     | int  | 主开关   | [SwitchState][SwitchState]                 |
| deposit  | int  | 充值开关 | [GrabSwitchOrderType][GrabSwitchOrderType] |
| withdraw | int  | 提现开关 | [GrabSwitchOrderType][GrabSwitchOrderType] |

## GrabSwitchOrderType

[GrabSwitchOrderType]:#GrabSwitchOrderType

> 抢单开关配置内部类,指定不同类型订单的开关状态

| 字段     | 类型 | 说明                   | 跳转                       |
| -------- | ---- | ---------------------- | -------------------------- |
| player   | int  | 接收来自玩家的订单开关 | [SwitchState][SwitchState] |
| merchant | int  | 接收来自商家的订单开关 | [SwitchState][SwitchState] |

# 配置业务枚举

## SwitchState

[SwitchState]:#SwitchState

> 开关状态枚举 0-关闭 1-开启

# 支付业务VO

## PaymentVo

[PaymentVo]:#PaymentVo

> 支付信息类型，继承自[GIIdentity][GIIdentity]<Long>

| 字段       | 类型   | 说明             | 跳转                         |
| ---------- | ------ | ---------------- | ---------------------------- |
| merchantId | long   | 商户ID           |                              |
| ownerName  | string | 持有人姓名       |                              |
| way        | string | 支付方式code     | [PayWay][PayWay]             |
| goal       | int    | 支付信息用途     | [PaymentGoal][PaymentGoal]   |
| qr         | object | 二维码信息       | [QrCode][QrCode]             |
| belong     | object | 支付信息所属机构 | [Belong][Belong]             |
| state      | int    | 支付信息状态     | [PaymentState][PaymentState] |
| ramark     | string | 备注信息         |                              |

## PaymentWay

[PaymentWay]: #PaymentWay

> 支付信息方式，继承自 [Property][Property]<String>
> code可用值见[PayWay][PayWay]

## QrCode

[QrCode]: #QrCode

> 二维码类型

| 字段  | 类型   | 说明                          | 跳转 |
| ----- | ------ | ----------------------------- | ---- |
| img   | string | 二维码图片地址                |      |
| link  | string | 二维码内含链接                |      |
| stamp | string | 二维码验签值\|目前使用MD5签名 |      |

## Belong

[Belong]: #Belong

> 收付款方式所属结构

| 字段  | 类型   | 说明     | 跳转 |
| ----- | ------ | -------- | ---- |
| major | string | 主要机构 |      |
| minor | string | 次要机构 |      |

# 支付业务枚举

## PayWay

[PayWay]:#PayWay

> 支付方式枚举，目前支持：bankcard-银行卡 | AliPay-支付宝 | WeChatPay-微信 

## PaymentGoal

[PaymentGoal]:#PaymentGoal

> 支付信息用途说明： 1-抢单支付 2-商户充提

## PaymentState

[PaymentState]:#PaymentState

> 支付信息状态：  1-开启 2-关闭 3-删除

# 商家业务VO

## MerchantVo

[MerchantVo]:#MerchantVo

> 商家信息类，继承自[GIIdentity][GIIdentity]<Long>



# 订单业务VO

## OrderVo

[OrderVo]:#OrderVo

> 订单信息类，继承自[GIIdentity][GIIdentity]<Long>

| 字段       | 类型   | 说明                                       | 跳转                               |
| ---------- | ------ | ------------------------------------------ | ---------------------------------- |
| property   | object | 订单的基础属性                             | [OrderProperty][OrderProperty]     |
| state      | object | 订单的状态                                 | [OrderState][OrderState]           |
| amount     | object | 订单的金额信息                             | [OrderAmount][OrderAmount]         |
| payInfo    | object | 订单的收款信息                             | [PaymentVo][PaymentVo]             |
| recvInfo   | object | 订单中使用的支付信息                       | [PaymentVo][PaymentVo]             |
| pttl       | long   | 订单自动关闭的超时时间,毫秒,null则忽略不计 |                                    |
| time       | object | 时间对                                     | [TimePair][TimePair]               |
| thirdParty | object | 第三方的订单信息                           | [ThirdPartyOrder][ThirdPartyOrder] |

## OrderProperty

[OrderProperty]:#OrderProperty

> 订单的基础属性

| 字段  | 类型 | 说明           | 跳转                   |
| ----- | ---- | -------------- | ---------------------- |
| type  | int  | 订单的类型     | [OrderType][OrderType] |
| style | int  | 订单的交易类型 | [DealType][DealType]   |

## OrderAmount

[OrderAmount]:#OrderAmount

> 订单金额类

| 字段    | 类型   | 说明       | 跳转                 |
| ------- | ------ | ---------- | -------------------- |
| expect  | number | 预期的金额 |                      |
| reality | number | 实际的金额 |                      |
| fee     | number | 手续费金额 |                      |
| income  | number | 收益的金额 |                      |
| unit    | object | 金额单位   | [Currency][Currency] |

## OrderState

[OrderState]:#OrderState

> 订单的状态类

| 字段 | 类型 | 说明           | 跳转                   |
| ---- | ---- | -------------- | ---------------------- |
| deal | int  | 订单的交易状态 | [DealState][DealState] |
| paid | int  | 订单的支付状态 | [PaidState][PaidState] |

## ThirdPartyOrder

[ThirdPartyOrder]:#ThirdPartyOrder

> 第三方订单信息

| 字段         | 类型   | 说明         | 跳转 |
| ------------ | ------ | ------------ | ---- |
| orderAccount | String | 第三方订单号 |      |



# 订单业务枚举

## OrderType

[OrderType]:#OrderType

> 订单类型  1-来自平台的订单  2-钻石支付内的商家订单

## DealType

[DealType]:#DealType

> 订单交易类型 1-充值 2-提现

## DealState

[DealState]:#DealState

> 订单的交易状态 1-进行中 2-已完成 3-已关闭

## PaidState

[PaidState]:#PaidState

> 订单的支付状态 1-未支付 2-足额已支付 3-不足额已支付 4-超额已支付

