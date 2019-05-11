# Table of Contents

* [更新记录](#更新记录)
* [全局约定](#全局约定)
  * [通用返回结构](#通用返回结构)
* [资金接口](#资金接口)
  * [1_1_商家查询可用资产](#1_1_商家查询可用资产)
    * [接口路径&请求方式](#接口路径请求方式)
    * [参数](#参数)
    * [返回参数](#返回参数)
      * [样例](#样例)
* [支付信息接口](#支付信息接口)
  * [2_1_支付信息列表](#2_1_支付信息列表)
    * [接口路径&请求方式](#接口路径请求方式-1)
    * [参数](#参数-1)
    * [返回值](#返回值)
      * [样例](#样例-1)
  * [2_2_添加一个支付信息](#2_2_添加一个支付信息)
    * [接口路径&请求方式&请求ContentType](#接口路径请求方式请求contenttype)
    * [参数](#参数-2)
    * [返回值](#返回值-1)
      * [样例](#样例-2)
  * [2_3_修改支付信息状态](#2_3_修改支付信息状态)
    * [接口路径&请求方式](#接口路径请求方式-2)
    * [参数](#参数-3)
    * [返回值](#返回值-2)
      * [样例](#样例-3)
  * [2_4_删除支付信息](#2_4_删除支付信息)
    * [接口路径&请求方式](#接口路径请求方式-3)
    * [参数](#参数-4)
    * [返回值](#返回值-3)
      * [样例](#样例-4)
* [商家订单接口](#商家订单接口)
  * [3_1_商户充值](#3_1_商户充值)
    * [接口路径&请求方式](#接口路径请求方式-4)
    * [参数](#参数-5)
    * [返回值](#返回值-4)
      * [样例](#样例-5)
  * [3_2_商户提现](#3_2_商户提现)
    * [接口路径&请求方式](#接口路径请求方式-5)
    * [参数](#参数-6)
    * [返回值](#返回值-5)
      * [样例](#样例-6)
  * [3_3_分页查询商户的订单列表](#3_3_分页查询商户的订单列表)
    * [接口路径&请求方式](#接口路径请求方式-6)
    * [参数](#参数-7)
    * [返回值](#返回值-6)
      * [样例](#样例-7)
  * [3_4_查看订单详情](#3_4_查看订单详情)
    * [接口路径&请求方式](#接口路径请求方式-7)
    * [参数](#参数-8)
    * [返回值](#返回值-7)
      * [样例](#样例-8)
  * [3_5_充值订单,取消充值](#3_5_充值订单取消充值)
    * [接口路径&请求方式](#接口路径请求方式-8)
    * [参数](#参数-9)
    * [返回值](#返回值-8)
      * [样例](#样例-9)
  * [3_6_充值订单,完成支付](#3_6_充值订单完成支付)
    * [接口路径&请求方式](#接口路径请求方式-9)
    * [参数](#参数-10)
    * [返回值](#返回值-9)
      * [样例](#样例-10)
* [抢单订单接口](#抢单订单接口)
  * [4_1_获取开关状态](#4_1_获取开关状态)
    * [接口路径&请求方式](#接口路径请求方式-10)
    * [参数](#参数-11)
    * [返回值](#返回值-10)
      * [样例](#样例-11)
  * [4_2_修改开关状态](#4_2_修改开关状态)
    * [接口路径&请求方式](#接口路径请求方式-11)
    * [参数](#参数-12)
    * [返回值](#返回值-11)
      * [样例](#样例-12)
  * [4_3_抢单](#4_3_抢单)
    * [接口路径&请求方式](#接口路径请求方式-12)
    * [参数](#参数-13)
    * [返回值](#返回值-12)
      * [样例](#样例-13)
  * [4_4_玩家充值订单商家确认支付](#4_4_玩家充值订单商家确认支付)
    * [接口路径&请求方式](#接口路径请求方式-13)
    * [参数](#参数-14)
    * [返回值](#返回值-13)
      * [样例](#样例-14)
  * [4_5_玩家提现订单商家确认收款](#4_5_玩家提现订单商家确认收款)
    * [接口路径&请求方式](#接口路径请求方式-14)
    * [参数](#参数-15)
    * [返回值](#返回值-14)
      * [样例](#样例-15)
  * [4_6_查询进行中的订单](#4_6_查询进行中的订单)
    * [接口路径&请求方式](#接口路径请求方式-15)
    * [参数](#参数-16)
    * [返回值](#返回值-15)
      * [样例](#样例-16)
  * [4_7_历史订单分页列表查询](#4_7_历史订单分页列表查询)
    * [接口路径&请求方式](#接口路径请求方式-16)
    * [参数](#参数-17)
    * [返回值](#返回值-16)
      * [样例](#样例-17)
  * [4_8_重新开启抢单并且设置本次收款信息](#4_8_重新开启抢单并且设置本次收款信息)
    * [接口路径&请求方式](#接口路径请求方式-17)
    * [参数](#参数-18)
    * [返回值](#返回值-17)
      * [样例](#样例-18)


# 更新记录

| 版本号  | 作者 | 日期       | 说明                                                         |
| ------- | ---- | ---------- | ------------------------------------------------------------ |
| v.2.0.0 | D    | 2019.05.09 | 初始版本                                                     |
| v.2.0.1 | D    | 2019.05.10 | 修改。3_5接口路径                                            |
| v.2.0.2 | D    | 2019.05.11 | 1.OrderVo删除owner字段；2.PaymentVo增加remark字段；3.修改GrabSwitch类结构；4.修改接口【4_2】入参；5.增加接口【4_8】 |



# 全局约定

## 通用返回结构

> 作为通用的返回结构，业务接口仅描述data数据结构。泛型类型是data的类型

| 字段    | 类型    | 说明                           | 跳转 |
| ------- | ------- | ------------------------------ | ---- |
| success | boolean | 业务执行结果状态标识 true-成功 |      |
| code    | int     | 业务执行结果code               |      |
| message | string  | 业务执行结果描述               |      |
| data    | T       | 业务返回的数据,详见各业务接口  |      |

```json
{
    "success": true,
    "code": 0,
    "message": "成功",
    "data": null
}
```



# 资金接口

## 1_1_商家查询可用资产

### 接口路径&请求方式

/merchant/assets/list GET

### 参数

| 字段 | 类型   | 是否必填 | 说明                             |
| ---- | ------ | -------- | -------------------------------- |
| code | String | 否       | 币种code。指定则查询时限定该条件 |

### 返回参数

> data是array类型，内部数据类型： [AssetVo][AssetVo]

#### 样例

``` json
{
	"code":0,
	"data":[
		{
			"currency":{
				"code":"CNY",
				"icon":"https://www.dc.pay.com/cny.icon",
				"name":"人民币",
				"precision":2,
				"symbol":"Y"
			},
			"free":99.99,
			"id":1000,
			"time":{
				"create":1557423631329,
				"modify":1557423631329
			},
			"unfree":0
		}
	],
    "message":"成功",
	"success":true
}

```



# 支付信息接口 

## 2_1_支付信息列表

### 接口路径&请求方式

/merchant/payment/list GET

### 参数

| 字段  | 类型   | 是否必填 | 说明                                | 跳转                         |
| ----- | ------ | -------- | ----------------------------------- | ---------------------------- |
| goal  | int    | 否       | 支付信息用途,指定则查询时限定该条件 | [PaymentGoal][PaymentGoal]   |
| state | int    | 否       | 支付信息状态,指定则查询时限定该条件 | [PaymentState][PaymentState] |
| way   | String | 否       | 支付方式code,指定则查询时限定该条件 | [PayWay][PayWay]             |

### 返回值

> data是array类型，内部数据类型： [PaymentVo][PaymentVo]

#### 样例

```json
{
	"code":0,
	"data":[
		{
			"account":"18888888888",
			"belong":{
				"major":"蚂蚁金融",
				"minor":"支付宝"
			},
			"goal":1,
			"id":1,
			"merchantId":10000,
			"ownerName":"张小三",
			"qr":{
				"img":"https://www.dc.pay.com/alipay.img",
				"link":"HTTPS://QR.ALIPAY.COM/XSDFS",
				"stamp":"lkmvnhgiyrnqkjfndkjhfakadsnfa"
			},
			"state":1,
			"way":"AliPay"
		}
	],
	"message":"成功",
	"success":true
}

```

## 2_2_添加一个支付信息

### 接口路径&请求方式&请求ContentType

/merchant/payment/add POST multipart/form-data

> 特殊请求内容类型，支持单张图片上传，图片信息以字节流方式上传
> 银行卡无需上传图片；支付宝\微信必须上传图片
> 银行卡必须输入主归属值(belong),作为主行；其他支付方式无需输入

### 参数

| 字段      | 类型   | 是否必填 | 说明         |跳转|
| --------- | ------ | -------- | ------------ |----|
| goal      | int    | 是       | 支付信息用途 |[PaymentGoal][PaymentGoal]|
| way       | string | 是       | 支付方式 |[PayWay][PayWay]|
| ownerName | string | 是       | 拥有者姓名 ||
| account   | string | 是 | 支付信息账号 ||
| remark | string | 否 | 备注\留言 ||
| belong    | string | 否       | 支付信息主归属结构 ||
| subBelong | string | 否       | 支付信息从归属结构 ||
| remark | string | 否 | 备注信息 ||
| vfcode | string | 是 | 手机短信验证码 ||

### 返回值

> data类型 [PaymentVo][PaymentVo],本次添加的支付信息

#### 样例

``` json
{
	"code":0,
	"data":{
		"account":"18888888888",
		"belong":{
			"major":"蚂蚁金融",
			"minor":"支付宝"
		},
		"goal":1,
		"id":1,
		"merchantId":10000,
		"ownerName":"张小三",
		"qr":{
			"img":"https://www.dc.pay.com/alipay.img",
			"link":"HTTPS://QR.ALIPAY.COM/XSDFS",
			"stamp":"lkmvnhgiyrnqkjfndkjhfakadsnfa"
		},
		"state":1,
		"way":"AliPay",
        "remark":"收款专用"
	},
	"message":"成功",
	"success":true
}

```

## 2_3_修改支付信息状态

### 接口路径&请求方式

/merchant/payment/turn POST

### 参数

| 字段  | 类型 | 是否必传 | 说明       | 跳转                         |
| ----- | ---- | -------- | ---------- | ---------------------------- |
| id    | long | 是       | 支付信息ID |                              |
| state | int  | 是       | 新状态值   | [PaymentState][PaymentState] |

### 返回值

> data无意义

#### 样例

```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```

## 2_4_删除支付信息

### 接口路径&请求方式

/merchant/payment/del POST

### 参数

| 字段 | 类型 | 是否必传 | 说明       | 跳转 |
| ---- | ---- | -------- | ---------- | ---- |
| id   | long | 是       | 支付信息ID |      |

### 返回值

> data无意义

#### 样例

```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```

# 商家订单接口 

## 3_1_商户充值

### 接口路径&请求方式

/merchant/order/deposit POST
### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|amount|number|是 |充值金额||
|payId|long|是 |付款信息ID||
### 返回值
> data类型[OrderVo][OrderVo],本次创建的订单
#### 样例
```json
{
	"code":0,
	"data":{
		"amount":{
			"expect":50000,
			"fee":0,
			"income":0,
			"reality":50000,
			"unit":{
				"code":"CNY",
				"icon":"https://www.dc.pay.com/cny.icon",
				"name":"人民币",
				"precision":2,
				"symbol":"Y"
			}
		},
		"payInfo":{
			"account":"622202048888909",
			"belong":{
				"major":"北京银行",
				"minor":"浪琴支行"
			},
			"goal":2,
			"id":100,
			"merchantId":100,
			"ownerName":"张小三",
			"state":1,
			"way":"bankcard"
		},
		"property":{
			"style":1,
			"type":2
		},
		"pttl":null,
		"recvInfo":{
			"account":"622202048888909",
			"belong":{
				"major":"北京银行",
				"minor":"浪琴支行"
			},
			"goal":2,
			"id":101,
			"merchantId":101,
			"ownerName":"张大三",
			"state":1,
			"way":"bankcard"
		},
		"state":{
			"deal":1,
			"paid":1
		},
		"time":{
			"create":1557453663693,
			"modify":1557453663694
		}
	},
	"message":"成功",
	"success":true
}

```

## 3_2_商户提现

### 接口路径&请求方式

/merchant/order/withdraw POST
### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|amount|number|是 |提现金额||
|recvId|long|是 |收款信息ID||
|feeRate|number|是 |展示给用户的手续费率||
|vfcode|string|是 |手机验证码||
### 返回值
> data类型[OrderVo][OrderVo],本次创建的订单
#### 样例
```json
{
	"code":0,
	"data":{
		"amount":{
			"expect":50000,
			"fee":0,
			"income":0,
			"reality":47500,
			"unit":{
				"code":"CNY",
				"icon":"https://www.dc.pay.com/cny.icon",
				"name":"人民币",
				"precision":2,
				"symbol":"Y"
			}
		},
		"property":{
			"style":2,
			"type":2
		},
		"pttl":null,
		"recvInfo":{
			"account":"622202048888909",
			"belong":{
				"major":"北京银行",
				"minor":"浪琴支行"
			},
			"goal":2,
			"id":100,
			"merchantId":100,
			"ownerName":"张小三",
			"state":1,
			"way":"bankcard"
		},
		"state":{
			"deal":1,
			"paid":1
		},
		"time":{
			"create":1557453821437,
			"modify":1557453821437
		}
	},
	"message":"成功",
	"success":true
}
```

## 3_3_分页查询商户的订单列表

### 接口路径&请求方式

/merchant/order/paging GET
### 参数

> 分页页码参数 [PaginationParam][PaginationParam]

### 返回值
> data类型 [Page][Page]<[OrderVo][OrderVo]>
#### 样例
```json
{
	"code":0,
	"data":{
		"content":[
			{
				"amount":{
					"expect":50000,
					"fee":0,
					"income":0,
					"reality":47500,
					"unit":{
						"code":"CNY",
						"icon":"https://www.dc.pay.com/cny.icon",
						"name":"人民币",
						"precision":2,
						"symbol":"Y"
					}
				},
				"payInfo":{
					"account":"622202048888909",
					"belong":{
						"major":"北京银行",
						"minor":"浪琴支行"
					},
					"goal":2,
					"id":100,
					"merchantId":100,
					"ownerName":"张小三",
					"state":1,
					"way":"bankcard"
				},
				"property":{
					"style":1,
					"type":1
				},
				"pttl":null,
				"recvInfo":{
					"account":"622202048888909",
					"belong":{
						"major":"北京银行",
						"minor":"浪琴支行"
					},
					"goal":2,
					"id":101,
					"merchantId":101,
					"ownerName":"张大三",
					"state":1,
					"way":"bankcard"
				},
				"state":{
					"deal":1,
					"paid":1
				},
				"thirdParty":null,
				"time":{
					"create":1557454924129,
					"modify":1557454924129
				}
			}
		],
		"pagination":{
			"num":1,
			"size":10,
			"total":200
		}
	},
	"message":"成功",
	"success":true
}
```

## 3_4_查看订单详情

### 接口路径&请求方式

/merchant/order/detail GET
### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|id|long|是 |订单ID||
### 返回值
> data类型[OrderVo][OrderVo]
#### 样例
```json
{
    "code": 0,
    "data": {
        "amount": {
            "expect": 50000,
            "fee": 0,
            "income": 0,
            "reality": 47500,
            "unit": {
                "code": "CNY",
                "icon": "https://www.dc.pay.com/cny.icon",
                "name": "人民币",
                "precision": 2,
                "symbol": "Y"
            }
        },
        "payInfo": {
            "account": "622202048888909",
            "belong": {
                "major": "北京银行",
                "minor": "浪琴支行"
            },
            "goal": 2,
            "id": 100,
            "merchantId": 100,
            "ownerName": "张小三",
            "state": 1,
            "way": "bankcard"
        },
        "property": {
            "style": 2,
            "type": 2
        },
        "pttl": null,
        "recvInfo": {
            "account": "622202048888909",
            "belong": {
                "major": "北京银行",
                "minor": "浪琴支行"
            },
            "goal": 2,
            "id": 101,
            "merchantId": 100,
            "ownerName": "张大三",
            "state": 1,
            "way": "bankcard"
        },
        "state": {
            "deal": 1,
            "paid": 1
        },
        "time": {
            "create": 1557454119285,
            "modify": 1557454119285
        }
    },
    "message": "成功",
    "success": true
}
```

## 3_5_充值订单,取消充值

### 接口路径&请求方式

/merchant/order/deposit/cancel POST
### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|id|long|是 |订单ID||
### 返回值
> data无意义
#### 样例
```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```

## 3_6_充值订单,完成支付

### 接口路径&请求方式

/merchant/order/deposit/pay POST

### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|id|long|是 |订单ID||
### 返回值
> data无意义
#### 样例
```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```

# 抢单订单接口

## 4_1_获取开关状态
### 接口路径&请求方式
/merchant/grab/switch GET
### 参数
无参数
### 返回值
> data类型[GrabSwitch][GrabSwitch]
#### 样例
```json
{
	"code":0,
	"data":{
		"deposit":{
        	"player":1,
            "merchant":1
        },
		"main":1,
        "withdraw":{
            "merchant":1
        }
	},
    "message":"成功",
	"success":true
}

```
## 4_2_修改开关状态
### 接口路径&请求方式
/merchant/grab/switch/turn POST

> 仅修改非null的入参配置

### 参数
|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|main| int|否|主开关状态|[SwitchState][SwitchState]|
|playerDeposit| int |否|玩家充值开关状态|[SwitchState][SwitchState]|
|playerWithdraw| int |否|玩家提现开关状态|[SwitchState][SwitchState]|
|merchantWithdraw| int |否|商家提现开关状态|[SwitchState][SwitchState]|
### 返回值
> data类型[GrabSwitch][GrabSwitch]，修改后的开关状态
#### 样例
```json
{
	"code":0,
	"data":{
		"deposit":{
        	"player":1,
            "merchant":1
        },
		"main":1,
        "withdraw":{
            "merchant":1
        }
	},
    "message":"成功",
	"success":true
}
```

## 4_3_抢单
### 接口路径&请求方式
/merchant/grab/grab POST
### 参数
|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|id| int|是|订单ID||
### 返回值
> data类型[OrderVo][OrderVo]，抢到的订单详情
#### 样例
```json
{
	"code":0,
	"data":{
		"amount":{
			"expect":50000,
			"fee":0,
			"income":0,
			"reality":47500,
			"unit":{
				"code":"CNY",
				"icon":"https://www.dc.pay.com/cny.icon",
				"name":"人民币",
				"precision":2,
				"symbol":"Y"
			}
		},
		"property":{
			"style":1,
			"type":1
		},
		"pttl":1800000,
		"recvInfo":{
			"account":"622202048888909",
			"belong":{
				"major":"蚂蚁金融",
				"minor":"支付宝"
			},
			"goal":1,
			"id":100,
			"merchantId":100,
			"ownerName":"张小三",
			"qr":{
				"img":"https://dc.pay.com/bankcard.img",
				"link":"HTTPS://QR.ALIPAY.COM/SIDNFDSE",
				"stamp":"wefdsdcvfasdfdtfsdfdssefg"
			},
			"state":1,
			"way":"AliPay",
            "remark":"张小三的支付宝"
		},
		"state":{
			"deal":1,
			"paid":1
		},
		"thirdParty":{
			"orderAccount":"TC20190510101054999SIENDFC"
		},
		"time":{
			"create":1557454545049,
			"modify":1557454545049
		}
	},
	"message":"成功",
	"success":true
}
```
## 4_4_玩家充值订单商家确认支付
### 接口路径&请求方式
/merchant/grab/pay POST
### 参数
|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|id| int|是|订单ID||
|amount| number|是|实际支付的金额||
### 返回值
> data无意义
#### 样例
```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```

## 4_5_玩家提现订单商家确认收款
### 接口路径&请求方式
/merchant/grab/recv POST
### 参数
|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|id| int|是|订单ID||
### 返回值
> data无意义
#### 样例
```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```

## 4_6_查询进行中的订单
### 接口路径&请求方式
/merchant/grab/inhand/list GET
### 参数
无参数
### 返回值
> data是array类型，内部数据类型： [OrderVo][OrderVo]
#### 样例
```json
{
	"code":0,
	"data":[
		{
			"amount":{
				"expect":50000,
				"fee":0,
				"income":0,
				"reality":47500,
				"unit":{
					"code":"CNY",
					"icon":"https://www.dc.pay.com/cny.icon",
					"name":"人民币",
					"precision":2,
					"symbol":"Y"
				}
			},
			"property":{
				"style":1,
				"type":1
			},
			"pttl":1800000,
			"recvInfo":{
				"account":"622202048888909",
				"belong":{
					"major":"蚂蚁金融",
					"minor":"支付宝"
				},
				"goal":1,
				"id":100,
				"merchantId":100,
				"ownerName":"张小三",
				"qr":{
					"img":"https://dc.pay.com/bankcard.img",
					"link":"HTTPS://QR.ALIPAY.COM/SIDNFDSE",
					"stamp":"wefdsdcvfasdfdtfsdfdssefg"
				},
				"state":1,
				"way":"AliPay",
          	    "remark":"张小三的支付宝"
			},
			"state":{
				"deal":2,
				"paid":2
			},
			"thirdParty":{
				"orderAccount":"TC20190510101054999SIENDFC"
			},
			"time":{
				"create":1557455835690,
				"modify":1557455835690
			}
		}
	],
	"message":"成功",
	"success":true
}

```

## 4_7_历史订单分页列表查询
### 接口路径&请求方式
/merchant/grab/past/paging GET
### 参数
> 继承自[PaginationParam][PaginationParam]

|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|state|  int | 否 | 订单状态,指定则查询时限定该条件|[DealState][DealState] |
### 返回值
> data数据类型： [Page][Page]<[OrderVo][OrderVo]>
#### 样例
```json
{
	"code":0,
	"data":{
		"content":[
			{
				"amount":{
					"expect":50000,
					"fee":0,
					"income":0,
					"reality":47500,
					"unit":{
						"code":"CNY",
						"icon":"https://www.dc.pay.com/cny.icon",
						"name":"人民币",
						"precision":2,
						"symbol":"Y"
					}
				},
				"property":{
					"style":1,
					"type":1
				},
				"pttl":1800000,
				"recvInfo":{
					"account":"622202048888909",
					"belong":{
						"major":"蚂蚁金融",
						"minor":"支付宝"
					},
					"goal":1,
					"id":100,
					"merchantId":100,
					"ownerName":"张小三",
					"qr":{
						"img":"https://dc.pay.com/bankcard.img",
						"link":"HTTPS://QR.ALIPAY.COM/SIDNFDSE",
						"stamp":"wefdsdcvfasdfdtfsdfdssefg"
					},
					"state":1,
					"way":"AliPay",
                    "remark":"张小三的支付宝"
				},
				"state":{
					"deal":2,
					"paid":2
				},
				"thirdParty":{
					"orderAccount":"TC20190510101054999SIENDFC"
				},
				"time":{
					"create":1557455368504,
					"modify":1557455368504
				}
			}
		],
		"pagination":{
			"num":1,
			"size":10,
			"total":200
		}
	},
	"message":"成功",
	"success":true
}
```

## 4_8_重新开启抢单并且设置本次收款信息

### 接口路径&请求方式

/merchant/grab/restart POST

### 参数

| 字段          | 类型  | 是否必填 | 说明                   | 跳转 |
| ------------- | ----- | -------- | ---------------------- | ---- |
| paymentIdList | array | 是       | 开启时选定的支付信息ID |      |

### 返回值
> data无意义
#### 样例
```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```



[PaginationParam]:vo.md#PaginationParam
[GIIdentity]:vo.md#GIIdentity
[Property]:vo.md#Property
[Currency]:vo.md#Currency
[TimePair]:vo.md#TimePair
[Pagination]:vo.md#Pagination
[Page]:vo.md#Page
[AssetVo]:vo.md#AssetVo
[GrabSwitch]:vo.md#GrabSwitch
[SwitchState]:vo.md#SwitchState
[PaymentVo]:vo.md#PaymentVo
[PaymentWay]:vo.md#PaymentWay
[QrCode]:vo.md#QrCode
[Belong]:vo.md#Belong
[PayWay]:vo.md#PayWay
[PaymentGoal]:vo.md#PaymentGoal
[PaymentState]:vo.md#PaymentState
[MerchantVo]:vo.md#MerchantVo
[OrderVo]:vo.md#OrderVo
[OrderProperty]:vo.md#OrderProperty
[OrderAmount]:vo.md#OrderAmount
[OrderState]:vo.md#OrderState
[ThirdPartyOrder]:vo.md#ThirdPartyOrder
[OrderType]:vo.md#OrderType
[DealType]:vo.md#DealType
[DealState]:vo.md#DealState
[PaidState]:vo.md#PaidState
