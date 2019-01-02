# 打赏他人



打赏 0.1 EOS 给他人



### HTTP

> POST /like_others



### 参数



| 名称    | 类型   | 必须？ | 默认值 | 说明       |
| ------- | ------ | ------ | ------ | ---------- |
| user_id | string | 是     | 无     | 被打赏的人 |



###返回

成功的返回

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "pay_url": "https://mixin.one/pay?recipient=faf9XXXX"
    }
}
```

