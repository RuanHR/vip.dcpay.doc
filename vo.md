[TOC]

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

## Situation

[Situation]:#Situation

> 状态描述类,泛型类型是value的类型

| 字段    | 类型   | 说明                              | 跳转 |
| ------- | ------ | --------------------------------- | ---- |
| state   | int    | 状态码,见具体业务说明             |      |
| value   | T      | 当前状态下附件的值,见具体业务说明 |      |
| explain | String | 状态的说明信息                    |      |

## Range<T>

[Range]:#Range

> 范围结构体，泛型类型是max,min的类型

| 字段 | 类型 | 说明   | 跳转 |
| ---- | ---- | ------ | ---- |
| max  | T    | 最大值 |      |
| min  | T    | 最小值 |      |



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

| 字段     | 类型   | 说明     | 跳转                                       |
| -------- | ------ | -------- | ------------------------------------------ |
| main     | int    | 主开关   | [SwitchState][SwitchState]                 |
| deposit  | object | 充值开关 | [GrabSwitchOrderType][GrabSwitchOrderType] |
| withdraw | int    | 提现开关 | [SwitchState][SwitchState]                 |

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
>
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

> 支付方式枚举，目前支持：Bankcard-银行卡 | AliPay-支付宝 | WechatPay-微信 

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

| 字段           | 类型   | 说明           | 跳转                             |
| -------------- | ------ | -------------- | -------------------------------- |
| uid            | String | 展示的ID       |                                  |
| auth           | object | 商家的认证信息 | [MerchantAuthVo][MerchantAuthVo] |
| invitationCode | String | 商家的邀请码   |                                  |
| type           | int    | 商家的类型     | [MerchantTpye][MerchantTpye]     |

## MerchantAuthVo

[MerchantAuthVo]:#MerchantAuthVo

> 商户认证Vo

| 字段  | 类型   | 说明                                                   | 跳转                                                       |
| ----- | ------ | ------------------------------------------------------ | ---------------------------------------------------------- |
| phone | object | 商家手机认证状态信息,[详见](#MerchantAuthVo_phone说明) | [Situation][Situation]<[PhoneNumber][PhoneNumber]>         |
| deal  | object | 商家交易状态信息,[详见](#MerchantAuthVo_deal说明)      | [Situation][Situation]<[ActivationFeeVo][ActivationFeeVo]> |

## MerchantAuthVo_phone说明

> 商家手机认证状态信息
>
> 一个[Situation][Situation]<PhoneNumber>结构:
>
> > phone.state可选值见[SwitchState][SwitchState]
>
> > phone.value认证后的手机号码,见[PhoneNumber][PhoneNumber]
>
> > phone.explain暂无意义

## PhoneNumber

[PhoneNumber]:#PhoneNumber

> 电话号码类型

| 字段 | 类型   | 说明                 | 跳转 |
| ---- | ------ | -------------------- | ---- |
| area | string | 国码                 |      |
| tel  | string | 电话号码（不含国码） |      |

## MerchantAuthVo_deal说明

> 商家交易状态信息
>
> 一个[Situation][Situation]<ActivationFeeVo>结构:
>
> > deal.state可选值见[MerchantActivateState][MerchantActivateState]
>
> > deal.value商家激活费用信息,详见[ActivationFeeVo][ActivationFeeVo]
>
> > deal.explain 当前状态的额外描述. 驳回时是驳回理由；禁用时是禁用理由

## ActivationFeeVo

[ActivationFeeVo]:#ActivationFeeVo

> 商家激活费用结构

| 字段  | 类型   | 说明               | 跳转                 |
| ----- | ------ | ------------------ | -------------------- |
| value | number | 激活费用值         |                      |
| unit  | object | 激活费用的币种单位 | [Currency][Currency] |

# 商家业务枚举

## MerchantActivateState

[MerchantActivateState]:#MerchantActivateState

> 商家激活状态
>
> > 1-未申请激活 2-申请激活后审批中 3-已激活,可交易 4-申请激活被驳回 5-被禁用,不可交易

## MerchantTpye

[MerchantTpye]:#MerchantTpye

> 商家的类型
>
> > 1-普通商家 2-批发商

# 订单业务VO

## OrderVo

[OrderVo]:#OrderVo

> 订单信息类，继承自[GIIdentity][GIIdentity]<String>

| 字段       | 类型   | 说明                                       | 跳转                               |
| ---------- | ------ | ------------------------------------------ | ---------------------------------- |
| property   | object | 订单的基础属性                             | [OrderProperty][OrderProperty]     |
| state      | object | 订单的状态                                 | [OrderState][OrderState]           |
| amount     | object | 订单的金额信息                             | [OrderAmount][OrderAmount]         |
| payInfo    | object | 订单中使用的支付信息                             | [PaymentVo][PaymentVo]             |
| recvInfo   | object | 订单的收款信息                       | [PaymentVo][PaymentVo]             |
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

> 订单的交易状态  ~~1-进行中(弃用)~~ 2-已完成 ~~3-已关闭(弃用)~~ 11-未匹配 12-已匹配 ~~13-已支付(弃用)~~ 14-已收款 31-已关闭 32-已取消

## PaidState

[PaidState]:#PaidState

> 订单的支付状态 1-未支付 2-足额已支付 3-不足额已支付 4-超额已支付

# 业务辅助VO

## DealConfig

[DealConfig]:#DealConfig

> 交易配置结构

| 字段      | 类型   | 说明           | 跳转                                       |
| --------- | ------ | -------------- | ------------------------------------------ |
| condition | object | 交易配置的条件 | [DealConfigCondition][DealConfigCondition] |
| value     | object | 交易配置的值   | [DealConfigValue][DealConfigValue]         |

## DealConfigCondition

[DealConfigCondition]:#DealConfigCondition

> 交易配置的条件结构

| 字段     | 类型   | 说明                 | 跳转                 |
| -------- | ------ | -------------------- | -------------------- |
| payWay   | String | 交易要使用的支付方式 | [PayWay][PayWay]     |
| dealType | int    | 交易类型             | [DealType][DealType] |

## DealConfigValue

[DealConfigValue]:#DealConfigValue

> 交易配置的值结构

| 字段  | 类型   | 说明         | 跳转                   |
| ----- | ------ | ------------ | ---------------------- |
| fee   | object | 手续费配置   | [FeeConfig][FeeConfig] |
| range | object | 交易金额范围 | [Range][Range]<Number> |

## FeeConfig

[FeeConfig]:#FeeConfig

> 交易手续费配置结构

| 字段 | 类型   | 说明           | 跳转 |
| ---- | ------ | -------------- | ---- |
| rate | Number | 手续费率       |      |
| min  | Number | 单笔最小手续费 |      |

# 业务辅助枚举

## BusinessCode

[BusinessCode]:#BusinessCode

> 业务code定义:
>
> > 2001 - 添加支付方式发送手机验证码
>
> > 3001 - 商家提现发送手机验证码
>
> > 5001 - 商家修改密码发送手机验证码
>
> > 6001 - 找回密码发送验证码
>
> > 6002 - 登录发送验证码
>
> > 6003 - 商家注册发送验证码

## AccountKind

[AccountKind]:#AccountKind

> 账号种类:
>
> > 1 - 手机号



