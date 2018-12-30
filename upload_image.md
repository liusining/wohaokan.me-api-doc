# 上传图片



上传图片，返回颜值计算分数



### HTTP

> POST /upload_image



### 参数

| 名称  | 类型 | 必须？ | 默认值 | 说明     |
| ----- | ---- | ------ | ------ | -------- |
| image | File | 是     | 无     | 人像照片 |



### 返回

**成功**

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "beauty": 98,
        "gender": "Female",
        "age": 23
    }
}
```



**图片不合格**

```json
{
    "status": 400,
    "msg": "未检测到人脸 / 有多张人脸",
    "result": {}
}
```

