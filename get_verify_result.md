# 取回活体验证结果



验证完成后，前端需要来这里取回验证结果



### HTTP

> GET /get_verify_result?biz_token=BIZ_TOKEN



### 参数

| 名称      | 类型      | 必须？ | 默认值 | 说明                       |
| --------- | --------- | ------ | ------ | -------------------------- |
| biz_token | url param | 是     | 无     | Face++ 跳转回时带有的 code |



### 返回

结果是成功的

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "url": "https://s3.ap-northeast-1.amazonaws.com/abcd.jpg",
        "beauty": 77.769,
        "gender": "Male",
        "age": 23
     }
}
```



结果是不成功的

```json
{
    "status": 400,
    "msg": "认证失败：PASS_LIVING_NOT_THE_SAME",
    "result": {
        "url": "https://s3.ap-northeast-1.amazonaws.com/abcd.jpg",
        "beauty": 77.769,
        "gender": "Male",
        "age": 23,
        "verify_url": "https://openapi.faceid.com/lite/v1/do/XXX"
    }
}
```

