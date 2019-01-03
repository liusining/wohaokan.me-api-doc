# 检查订单是否支付完成



`POST api.mixin.one/payment` 返回 `status: paid` 之后，后端需要再检查一遍订单支付情况。如果成功，则返回用户的 mixin id



### HTTP



> POST /check_order



### 参数

| 名称     | 类型   | 必须？ | 默认值 | 说明     |
| -------- | ------ | ------ | ------ | -------- |
| trace_id | string | 是     | 无     | 订单编号 |



### 返回



支付成功

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "mixin_id": "30450981"
    }
}
```



支付不成功

```json
{
    "status": 400,
    "msg": "支付不成功",
    "result": {}
}
```

