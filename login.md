# 授权登录



用 mixin 返回的 code 来登录。



### HTTP

> GET /login?code=<mixin-code>



### 参数

| 名称 | 类型      | 必须？ | 默认值 | 说明              |
| ---- | --------- | ------ | ------ | ----------------- |
| code | url param | 是     | 无     | mixin 返回的 code |



### 返回

**成功**

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "name": "James Zhang"
    }
}
```



**失败**

```json
{
    "status": 400,
    "msg": "授权登录失败"
}
```

