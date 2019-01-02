# 查看喜欢的用户



点击 ❤️ 后，得到这些信息



### HTTP

> GET /users/:USER_ID



### 参数

| 名称    | 类型   | 必须？ | 默认值 | 说明                 |
| ------- | ------ | ------ | ------ | -------------------- |
| user_id | string | 是     | 无     | user_id, 拼在 url 中 |



### 返回



成功的返回

```json
{
  "status": 200,
  "msg": "OK",
  "result": {
    "name": "James Zhang",
    "age": 23,
    "likes": 12,
    "description": "I'm fine"
  }
}
```



