# 更新个人照片

在个人主页更新照片时，用这个接口

### HTTP

> POST /update_image

### 参数

| 名称  | 类型 | 必须？ | 默认值 | 说明                         |
| ----- | ---- | ------ | ------ | ---------------------------- |
| image | File | 是     | 无     | 用户要更新的照片，后端会 1:1 |

### 返回

更新成功

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "beauty": 98,
        "gender": "Female",
        "age": 23,
        "new_url": "https://example.com/abcd.jpg"
    }
}
```



更新不成功



```json
{
    "status": 400,
    "msg": "和之前的照片不是同一个人",
    "result": {}
}
```

