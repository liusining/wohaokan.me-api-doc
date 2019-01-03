# 打赏他人



打赏 0.1 EOS 给他人



### HTTP

> POST /like_others



### 参数



| 名称    | 类型   | 必须？ | 默认值 | 说明       |
| ------- | ------ | ------ | ------ | ---------- |
| user_id | string | 是     | 无     | 被打赏的人 |



### 返回

成功的返回

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "pay_url": "https://mixin.one/pay?recipient=faf9XXXX",
        "amount": 0.1,
        "asset_id": "6cfe566e-4aad-470b-8c9a-2fd35b49c68d",
        "opponent_id": "faf9c343-677e-4f84-89cd-4c5688f22f7c",
        "trace_id": "3b6ecdc6-0ebe-11e9-acf4-0242f3b5db4d"
  }
}
```

请求 pay_url 后，循环请求 `https://api.mixin.one/payments`, 参数取上面返回中的后四组参数，形式如下：

```json
{
    "amount": 0.1,
    "asset_id": "6cfe566e-4aad-470b-8c9a-2fd35b49c68d",
    "opponent_id": "faf9c343-677e-4f84-89cd-4c5688f22f7c",
    "trace_id": "3b6ecdc6-0ebe-11e9-acf4-0242f3b5db4d"
}
```


**没有权限**


```json
{
    "status": 400,
    "msg": "您未对我们授权支付功能，暂时无法打赏",
    "result": {}
}
```
