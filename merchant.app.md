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
  * [3_5_充值订单-取消充值](#3_5_充值订单-取消充值)
    * [接口路径&请求方式](#接口路径请求方式-8)
    * [参数](#参数-9)
    * [返回值](#返回值-8)
      * [样例](#样例-9)
  * [3_6_充值订单-完成支付](#3_6_充值订单-完成支付)
    * [接口路径&请求方式](#接口路径请求方式-9)
    * [参数](#参数-10)
    * [返回值](#返回值-9)
      * [样例](#样例-10)
  * [3_7_订单交易配置](#3_7_订单交易配置)
    * [接口路径&请求方式](#接口路径请求方式-10)
    * [参数](#参数-11)
    * [返回值](#返回值-10)
      * [样例](#样例-11)
  * [3_8_提现订单-确认收款](#3_8_提现订单-确认收款)
    * [接口路径&请求方式](#接口路径请求方式-11)
    * [参数](#参数-12)
    * [返回值](#返回值-11)
      * [样例](#样例-12)
* [抢单订单接口](#抢单订单接口)
  * [4_1_获取开关状态](#4_1_获取开关状态)
    * [接口路径&请求方式](#接口路径请求方式-12)
    * [参数](#参数-13)
    * [返回值](#返回值-12)
      * [样例](#样例-13)
  * [4_2_修改开关状态](#4_2_修改开关状态)
    * [接口路径&请求方式](#接口路径请求方式-13)
    * [参数](#参数-14)
    * [返回值](#返回值-13)
      * [样例](#样例-14)
  * [4_3_抢单](#4_3_抢单)
    * [接口路径&请求方式](#接口路径请求方式-14)
    * [参数](#参数-15)
    * [返回值](#返回值-14)
      * [样例](#样例-15)
  * [4_4_充值类型订单,商家确认收款](#4_4_充值类型订单商家确认收款)
    * [接口路径&请求方式](#接口路径请求方式-15)
    * [参数](#参数-16)
    * [返回值](#返回值-15)
      * [样例](#样例-16)
  * [4_5_提现类型订单,商家确认支付](#4_5_提现类型订单商家确认支付)
    * [接口路径&请求方式](#接口路径请求方式-16)
    * [参数](#参数-17)
    * [返回值](#返回值-16)
      * [样例](#样例-17)
  * [4_6_查询进行中的订单](#4_6_查询进行中的订单)
    * [接口路径&请求方式](#接口路径请求方式-17)
    * [参数](#参数-18)
    * [返回值](#返回值-17)
      * [样例](#样例-18)
  * [4_7_历史订单分页列表查询](#4_7_历史订单分页列表查询)
    * [接口路径&请求方式](#接口路径请求方式-18)
    * [参数](#参数-19)
      * [4_7_state说明](#4_7_state说明)
    * [返回值](#返回值-18)
      * [样例](#样例-19)
  * [4_8_重新开启抢单并且设置本次收款信息](#4_8_重新开启抢单并且设置本次收款信息)
    * [接口路径&请求方式](#接口路径请求方式-19)
    * [参数](#参数-20)
    * [返回值](#返回值-19)
      * [样例](#样例-20)
  * [4_9_商家查看领取到的订单详情](#4_9_商家查看领取到的订单详情)
    * [接口路径&请求方式](#接口路径请求方式-20)
    * [参数](#参数-21)
    * [返回值](#返回值-20)
      * [样例](#样例-21)
* [商家辅助接口](#商家辅助接口)
  * [5_1_获取商家个人信息](#5_1_获取商家个人信息)
    * [接口路径&请求方式](#接口路径请求方式-21)
    * [参数](#参数-22)
    * [返回值](#返回值-21)
      * [样例](#样例-22)
  * [5_2_商家发送验证码](#5_2_商家发送验证码)
    * [接口路径&请求方式](#接口路径请求方式-22)
    * [参数](#参数-23)
    * [返回值](#返回值-22)
      * [样例](#样例-23)
  * [5_3_修改密码](#5_3_修改密码)
    * [接口路径&请求方式](#接口路径请求方式-23)
    * [参数](#参数-24)
    * [返回值](#返回值-23)
      * [样例](#样例-24)
  * [5_4_查询激活费用配置](#5_4_查询激活费用配置)
    * [接口路径&请求方式](#接口路径请求方式-24)
    * [参数](#参数-25)
    * [返回值](#返回值-24)
      * [样例](#样例-25)
  * [5_5_申请激活账户](#5_5_申请激活账户)
    * [接口路径&请求方式](#接口路径请求方式-25)
    * [参数](#参数-26)
    * [返回值](#返回值-25)
      * [样例](#样例-26)
* [其他辅助接口](#其他辅助接口)
  * [6_1_未登录发送验证码](#6_1_未登录发送验证码)
    * [接口路径&请求方式](#接口路径请求方式-26)
    * [参数](#参数-27)
      * [6_1_params_account说明](#6_1_params_account说明)
    * [返回值](#返回值-26)
      * [样例](#样例-27)
  * [6_2_找回密码](#6_2_找回密码)
    * [接口路径&请求方式](#接口路径请求方式-27)
    * [参数](#参数-28)
      * [6_2_params_account说明](#6_2_params_account说明)
    * [返回值](#返回值-27)
      * [样例](#样例-28)
  * [6_3_登录接口](#6_3_登录接口)
    * [接口路径&请求方式](#接口路径请求方式-28)
    * [参数](#参数-29)
      * [6_3_params_account说明](#6_3_params_account说明)
    * [返回值](#返回值-28)
      * [样例](#样例-29)
  * [6_4_注册接口](#6_4_注册接口)
    * [接口路径&请求方式](#接口路径请求方式-29)
    * [参数](#参数-30)
      * [6_4_params_account说明](#6_4_params_account说明)
    * [返回值](#返回值-29)
  * [6_5_查询邀请链接的域名](#6_5_查询邀请链接的域名)
    * [接口路径&请求方式](#接口路径请求方式-30)
    * [参数](#参数-31)
    * [返回值](#返回值-30)
      * [样例](#样例-30)
* [查询代理接口](#查询代理接口)
  * [7_1_查询我的直属下级列表](#7_1_查询我的直属下级列表)
    * [接口路径&请求方式](#接口路径请求方式-31)
    * [返回参数](#返回参数-1)
      * [样例](#样例-31)
  * [7_2_搜索下级结果](#7_2_搜索下级结果)
    * [接口路径&请求方式](#接口路径请求方式-32)
    * [参数](#参数-32)
    * [返回参数](#返回参数-2)
      * [样例](#样例-32)


Table of Contents

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
  * [3_7_订单交易配置](#3_7_订单交易配置)
    * [接口路径&请求方式](#接口路径请求方式-10)
    * [参数](#参数-11)
    * [返回值](#返回值-10)
      * [样例](#样例-11)
* [抢单订单接口](#抢单订单接口)
  * [4_1_获取开关状态](#4_1_获取开关状态)
    * [接口路径&请求方式](#接口路径请求方式-11)
    * [参数](#参数-12)
    * [返回值](#返回值-11)
      * [样例](#样例-12)
  * [4_2_修改开关状态](#4_2_修改开关状态)
    * [接口路径&请求方式](#接口路径请求方式-12)
    * [参数](#参数-13)
    * [返回值](#返回值-12)
      * [样例](#样例-13)
  * [4_3_抢单](#4_3_抢单)
    * [接口路径&请求方式](#接口路径请求方式-13)
    * [参数](#参数-14)
    * [返回值](#返回值-13)
      * [样例](#样例-14)
  * [4_4_充值类型订单,商家确认收款](#4_4_充值类型订单商家确认收款)
    * [接口路径&请求方式](#接口路径请求方式-14)
    * [参数](#参数-15)
    * [返回值](#返回值-14)
      * [样例](#样例-15)
  * [4_5_提现类型订单,商家确认支付](#4_5_提现类型订单商家确认支付)
    * [接口路径&请求方式](#接口路径请求方式-15)
    * [参数](#参数-16)
    * [返回值](#返回值-15)
      * [样例](#样例-16)
  * [4_6_查询进行中的订单](#4_6_查询进行中的订单)
    * [接口路径&请求方式](#接口路径请求方式-16)
    * [参数](#参数-17)
    * [返回值](#返回值-16)
      * [样例](#样例-17)
  * [4_7_历史订单分页列表查询](#4_7_历史订单分页列表查询)
    * [接口路径&请求方式](#接口路径请求方式-17)
    * [参数](#参数-18)
      * [4_7_state说明](#4_7_state说明)
    * [返回值](#返回值-17)
      * [样例](#样例-18)
  * [4_8_重新开启抢单并且设置本次收款信息](#4_8_重新开启抢单并且设置本次收款信息)
    * [接口路径&请求方式](#接口路径请求方式-18)
    * [参数](#参数-19)
    * [返回值](#返回值-18)
      * [样例](#样例-19)
* [商家辅助接口](#商家辅助接口)
  * [5_1_获取商家个人信息](#5_1_获取商家个人信息)
    * [接口路径&请求方式](#接口路径请求方式-19)
    * [参数](#参数-20)
    * [返回值](#返回值-19)
      * [样例](#样例-20)
  * [5_2_商家发送验证码](#5_2_商家发送验证码)
    * [接口路径&请求方式](#接口路径请求方式-20)
    * [参数](#参数-21)
    * [返回值](#返回值-20)
      * [样例](#样例-21)
  * [5_3_修改密码](#5_3_修改密码)
    * [接口路径&请求方式](#接口路径请求方式-21)
    * [参数](#参数-22)
    * [返回值](#返回值-21)
      * [样例](#样例-22)
  * [5_4_查询激活费用配置](#5_4_查询激活费用配置)
    * [接口路径&请求方式](#接口路径请求方式-22)
    * [参数](#参数-23)
    * [返回值](#返回值-22)
      * [样例](#样例-23)
  * [5_5_申请激活账户](#5_5_申请激活账户)
    * [接口路径&请求方式](#接口路径请求方式-23)
    * [参数](#参数-24)
    * [返回值](#返回值-23)
      * [样例](#样例-24)
* [其他辅助接口](#其他辅助接口)
  * [6_1_未登录发送验证码](#6_1_未登录发送验证码)
    * [接口路径&请求方式](#接口路径请求方式-24)
    * [参数](#参数-25)
      * [6_1_params_account说明](#6_1_params_account说明)
    * [返回值](#返回值-24)
      * [样例](#样例-25)
  * [6_2_找回密码](#6_2_找回密码)
    * [接口路径&请求方式](#接口路径请求方式-25)
    * [参数](#参数-26)
      * [6_2_params_account说明](#6_2_params_account说明)
    * [返回值](#返回值-25)
      * [样例](#样例-26)
  * [6_3_登录接口](#6_3_登录接口)
    * [接口路径&请求方式](#接口路径请求方式-26)
    * [参数](#参数-27)
      * [6_3_params_account说明](#6_3_params_account说明)
    * [返回值](#返回值-26)
      * [样例](#样例-27)
  * [6_4_注册接口](#6_4_注册接口)
    * [接口路径&请求方式](#接口路径请求方式-27)
    * [参数](#参数-28)
      * [6_4_params_account说明](#6_4_params_account说明)
    * [返回值](#返回值-27)
* [查询代理接口](#查询代理接口)
  * [7_1_查询我的直属下级列表](#7_1_查询我的直属下级列表)
    * [接口路径&请求方式](#接口路径请求方式-1)
    * [参数](#参数)
    * [返回值](#返回值)
      * [样例](#样例)
  * [7_2_搜索下级结果](#7_2_搜索下级结果)
    * [接口路径&请求方式&请求ContentType](#接口路径请求方式请求contenttype)
    * [参数](#参数)
    * [返回值](#返回值)
      * [样例](#样例)

# 更新记录

| 版本号   | 作者 | 日期       | 说明                                                         |
| -------- | ---- | ---------- | ------------------------------------------------------------ |
| v.2.0.0  | D    | 2019.05.09 | 初始版本                                                     |
| v.2.0.10 | D    | 2019.06.12 | 修改 [DealState][DealState] 定义，增加 [BusinessCode][BusinessCode] 的定义 |
| v.2.0.11 | D    | 2019.06.12 | 增加接口 3_7_订单交易配置                                    |
| v.2.0.12 | D    | 2019.06.12 | 增加接口 4_9_商家查看领取到的订单详情                        |
| v.2.0.13 | D    | 2019.06.13 | 增加接口3_8_提现订单,确认收款                                |
| v.2.0.14 | Z    | 2019.06.13 | 增加接口7.1\|7.2 查询直属下级\|搜索下级结果                  |
| v.2.1.0  | D    | 2019.06.22 | 增加接口 6_5_查询邀请链接的域名                              |



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
>
> 银行卡无需上传图片；支付宝\微信必须上传图片
>
> 银行卡必须输入主归属值(belong),作为主行；其他支付方式无需输入

### 参数

| 字段      | 类型   | 是否必填 | 说明         |跳转|
| --------- | ------ | -------- | ------------ |----|
| goal      | int    | 是       | 支付信息用途 |[PaymentGoal][PaymentGoal]|
| way       | string | 是       | 支付方式 |[PayWay][PayWay]|
| ownerName | string | 是       | 拥有者姓名 ||
| account   | string | 是 | 支付信息账号 ||
| file | byte[] | 否 | 二维码图片字节流 ||
| belong    | string | 否       | 支付信息主归属结构 ||
| subBelong | string | 否       | 支付信息从归属结构 ||
| remark | string | 否 | 备注\留言 ||
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
|tradeAmount|number|是 |充值金额||
| knowGotAmount | number | 是       | 用户预期得到的金额 ||
| currency      | string | 是       | 充值币种           ||
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
|tradeAmount|number|是 |提现金额||
| knowGotAmount | number | 是       | 用户预期得到的金额 ||
| currency      | string | 是       | 提现币种           ||
|recvId|long|是 |收款信息ID||
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
|id|String|是 |订单ID||
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

## 3_5_充值订单-取消充值

### 接口路径&请求方式

/merchant/order/deposit/cancel POST
### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|id|String|是 |订单ID||
|reason|String|否 |取消理由||
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

## 3_6_充值订单-完成支付

### 接口路径&请求方式

/merchant/order/deposit/pay POST

### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|id|String|是 |订单ID||
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

## 3_7_订单交易配置

### 接口路径&请求方式

/merchant/order/config

### 参数

无

### 返回值

> data类型 List<[DealConfig][DealConfig]>

#### 样例

``` json
{
  "success": true,
  "code": 0,
  "message": "获取成功",
  "data": [
    {
      "condition": {
        "payWay": "Bankcard",
        "dealType": 1
      },
      "value": {
        "fee": {
          "rate": 0.03,
          "min": 100
        },
        "range": {
          "min": 3000,
          "max": 10000
        }
      }
    }
  ]
}
```

## 3_8_提现订单-确认收款

### 接口路径&请求方式

/merchant/order/withdraw/recv POST

### 参数
| 字段 | 类型 | 是否必传 | 说明 |跳转 |
|---- |----| ----|----|----|
|id|String|是 |订单ID||
|recvAmount|Number|是 |订单的交易金额||
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
[4_1]:#4_1_获取开关状态

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
        "withdraw":1
	},
    "message":"成功",
	"success":true
}

```
## 4_2_修改开关状态
[4_2]:#4_2_修改开关状态

### 接口路径&请求方式

/merchant/grab/switch/turn POST

> 仅修改非null的入参配置

### 参数
|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|main| int|否|主开关状态|[SwitchState][SwitchState]|
|playerDeposit| int |否|接收玩家充值订单开关状态|[SwitchState][SwitchState]|
|merchantDeposit| int |否|接收商家充值订单开关状态|[SwitchState][SwitchState]|
|withdraw| int |否|接收提现订单开关状态|[SwitchState][SwitchState]|
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
        "withdraw":1
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
|id| String |是|订单ID||
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
## 4_4_充值类型订单,商家确认收款
### 接口路径&请求方式
/merchant/grab/recv POST
### 参数
|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|id| String |是|订单ID||
|amount| number|是|实际收到的金额||
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

## 4_5_提现类型订单,商家确认支付
### 接口路径&请求方式
/merchant/grab/pay POST
### 参数
|字段 | 类型 | 是否必传 | 说明 | 跳转 |
|----|----|----|----|----|
|id| String |是|订单ID||
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
|state|  int | 否 | 订单状态,指定则查询时限定该条件|[详见:4_7_state说明](#4_7_state说明) |
#### 4_7_state说明

> 可用值 2-查询已完成订单，3-查询已关闭订单 ，不指定-查询已完成和已关闭的订单

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

## 4_9_商家查看领取到的订单详情

### 接口路径&请求方式

merchant/grab/detail GET

### 参数

| 字段 | 类型   | 是否必填 | 说明   | 跳转 |
| ---- | ------ | -------- | ------ | ---- |
| id   | string | 是       | 订单号 |      |

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



# 商家辅助接口

## 5_1_获取商家个人信息

### 接口路径&请求方式

/merchant/personal/info

### 参数

无参数

### 返回值

> data类型[MerchantVo][MerchantVo]

#### 样例

```json
{
	"account":"18888888888",
	"auth":{
		"deal":{
			"explain":"未申请激活状态",
			"state":1,
			"value":{
				"unit":{
					"code":"CNY",
					"precision":2
				},
				"value":0
			}
		},
		"phone":{
			"state":1,
			"value":{
				"area":"86",
				"tel":"18888888888"
			}
		}
	},
	"id":1000,
	"invitationCode":"stfc4",
	"type":2,
	"uid":"2900909"
}
```

## 5_2_商家发送验证码

### 接口路径&请求方式

/merchant/authcode/send POST

### 参数

| 字段         | 类型 | 是否必填 | 说明     | 跳转                         |
| ------------ | ---- | -------- | -------- | ---------------------------- |
| businessCode | int  | 是       | 业务编号 | [BusinessCode][BusinessCode] |

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

## 5_3_修改密码

### 接口路径&请求方式

/merchant/passwd/reset POST

### 参数

| 字段      | 类型   | 是否必填 | 说明           | 跳转 |
| --------- | ------ | -------- | -------------- | ---- |
| oldPasswd | string | 是       | 原密码         |      |
| newPasswd | string | 是       | 新密码         |      |
| vfcode    | string | 是       | 手机短信验证码 |      |

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

## 5_4_查询激活费用配置

[5_4]:#5_4_查询激活费用配置

### 接口路径&请求方式

/merchant/activation/fee GET

### 参数

无

### 返回值

> data 类型 [ActivationFeeVo][ActivationFeeVo]

#### 样例

```json
{
	"code":0,
	"data":{
		"unit":{
			"code":"CNY",
			"precision":2
		},
		"value":300
	},
	"message":"获取成功",
	"success":true
}
```

## 5_5_申请激活账户

[5_5]:#5_5_申请激活账户

### 接口路径&请求方式

/merchant/activation/apply POST

### 参数

| 字段     | 类型   | 是否必填 | 说明               |
| -------- | ------ | -------- | ------------------ |
| feeValue | number | 是       | 激活费用的值       |
| feeUnit  | string | 是       | 激活费用的币种code |

### 返回值

> data类型[MerchantVo][MerchantVo]. 激活成功后新的商户信息

#### 样例

> 见[5_1_获取商家个人信息:样例](#样例-19)



# 其他辅助接口

## 6_1_未登录发送验证码

### 接口路径&请求方式

/authcode/send POST

### 参数

| 字段         | 类型   | 是否必填 | 说明                   | 跳转                                   |
| ------------ | ------ | -------- | ---------------------- | -------------------------------------- |
| account      | string | 是       | 接收验证码的账号       | [account说明](#6_1_params_account说明) |
| accountKind  | int    | 是       | 接收验证码的账号的种类 | [AccountKind][AccountKind]             |
| businessCode | int    | 是       | 业务编号               | [BusinessCode][BusinessCode]           |

#### 6_1_params_account说明

>若账号种类是手机号，请传入完整号码,英标逗号分割，例如: "86,18888888888"

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

## 6_2_找回密码

### 接口路径&请求方式

/passwd/retrieval POST

### 参数

| 字段        | 类型   | 是否必填 | 说明                   | 跳转                                   |
| ----------- | ------ | -------- | ---------------------- | -------------------------------------- |
| account     | string | 是       | 接收验证码的账号       | [account说明](#6_2_params_account说明) |
| accountKind | int    | 是       | 接收验证码的账号的种类 | [AccountKind][AccountKind]             |
| passwd      | string | 是       | 新密码(MD5加密后)      |                                        |
| vfcode      | string | 是       | 手机短信验证码         |                                        |

#### 6_2_params_account说明

> 若账号种类是手机号，请传入完整号码,英标逗号分割，例如:"86,18888888888"

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

## 6_3_登录接口

### 接口路径&请求方式

/login POST

### 参数

| 字段        | 类型   | 是否必填 | 说明                   | 跳转                                   |
| ----------- | ------ | -------- | ---------------------- | -------------------------------------- |
| account     | string | 是       | 接收验证码的账号       | [account说明](#6_3_params_account说明) |
| accountKind | int    | 是       | 接收验证码的账号的种类 | [AccountKind][AccountKind]             |
| passwd      | string | 是       | 密码(MD5加密后)        |                                        |
| vfcode      | string | 是       | 手机短信验证码         |                                        |

#### 6_3_params_account说明

> 若账号种类是手机号，请传入完整号码,英标逗号分割，例如:"86,18888888888"

### 返回值

> data类型[MerchantVo][MerchantVo].本次登录的商家当前信息

> 登录成功响应头中返回本次登录的身份信息：utoken - 用户唯一身份标识；ttoken-随机token,每次登录后更新。utoken,ttoken在后续操作中带入到请求头中,作为身份标识

#### 样例

```http
HTTP/1.1 200 OK
Server: Tengine
Date: Mon, 13 May 2019 02:11:46 GMT
Content-Type: application/json;charset=UTF-8
utoken: E1449C64151030801DF5233ADC2D6A829C36FD15E786B7412A4EB61CECDCE421
ttoken: 17cd20ddcb55420980774d2eddfd3c14
X-Cache: MISS from kp4
Transfer-Encoding: chunked
Connection: keep-alive
```

> RESPONSE BODY 见[5_1_获取商家个人信息:样例](#样例-19)



##  6_4_注册接口

### 接口路径&请求方式

/signup POST

### 参数

| 字段           | 类型   | 是否必填 | 说明                   | 跳转                                   |
| -------------- | ------ | -------- | ---------------------- | -------------------------------------- |
| account        | string | 是       | 接收验证码的账号       | [account说明](#6_4_params_account说明) |
| accountKind    | int    | 是       | 接收验证码的账号的种类 | [AccountKind][AccountKind]             |
| invitationCode | string | 是       | 上级商家邀请码         |                                        |
| passwd         | string | 是       | 密码(MD5加密后)        |                                        |
| vfcode         | string | 是       | 手机短信验证码         |                                        |

#### 6_4_params_account说明

> 若账号种类是手机号，请传入完整号码,英标逗号分割，例如:"86,18888888888"

### 返回值

> data无意义

```json
{
	"code":0,
	"data":null,
	"message":"成功",
	"success":true
}
```

## 6_5_查询邀请链接的域名

### 接口路径&请求方式

/config/domain/invitation GET

### 参数

无

### 返回值

> data类型 String, 作为邀请链接的域名

#### 样例

```json
{
  "success": true,
  "code": 0,
  "message": "查询成功",
  "data": "https://www.baidu.com/1"
}
```



# 查询代理接口

## 7_1_查询我的直属下级列表

### 接口路径&请求方式

/merchant/agent/list GET

### 返回参数

| 字段               | 类型    | 说明     |
| ------------------ | ------- | -------- |
| merchantId         | Long    | 商户ID   |
| account            | String  | 账号     |
| teamCount          | Integer | 团队人数 |
| directlyUnderCount | Integer | 直属人数 |
| parentId           | Long    | 父ID     |



#### 样例

``` json
{
  "success": true,
  "code": 0,
  "message": "successful",
  "data": [
    {
      "merchantId": 2,
      "account": "17777777777",
      "teamCount": 0,
      "directlyUnderCount": 0,
      "parentId": 1
    },
    {
      "merchantId": 3,
      "account": "18888888888",
      "teamCount": 16,
      "directlyUnderCount": 12,
      "parentId": 1
    }
  ]
}

```
## 7_2_搜索下级结果

### 接口路径&请求方式

/merchant/agent/findByAccount GET

### 参数

| 字段        | 类型   | 是否必填 | 说明                   | 跳转                                   |
| ----------- | ------ | -------- | ---------------------- | -------------------------------------- |
| account     | string | 是       | 登陆的账号       | [account说明](#6_3_params_account说明) |
### 返回参数

#### 样例

``` json
{
  "success": true,
  "code": 0,
  "message": "successful",
  "data": {
    "merchantId": null,
    "account": "18888888888",
    "teamCount": 16,
    "directlyUnderCount": 12,
    "parentId": null
  }
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
[BusinessCode]:vo.md#BusinessCode
[AccountKind]: vo.md#AccountKind

[ActivationFeeVo]:vo.md#ActivationFeeVo
[DealConfig]:vo.md#DealConfig

