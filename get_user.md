# 获得用户信息



得到用户的全面信息



### HTTP

> GET /get_user



### 参数

不需要，有 cookie 行



### 返回

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "name": "James Zhang",
        "description": "I'm a frontend developer"
        "image": "https://example.com/abc.jpg",
        "beauty": 98,
        "gender": "Female",
        "age": 23,
        "rank": 14,
        "income": 0.1,
        "tip_transactions": {
            "count": 5,
            "to_boy": 3,
            "to_girl": 2
        }
    }
}
```



