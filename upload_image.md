# 上传图片



上传图片，返回颜值计算分数



### HTTP

> POST /upload_image



### 参数

| 名称  | 类型 | 必须？ | 默认值 | 说明         |
| ----- | ---- | ------ | ------ | ------------ |
| image | File | 是     | 无     | 传入人像照片 |



### 返回

**成功**

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "beauty": 98,
        "gender": "Female",
        "age": 23,
        "verify_url": "https://openapi.faceid.com/lite/v1/do/hahaha12312312"
    }
}
```

说明：
1. gender 有两种值，`"Female"` 和 `"Male"`


**图片不合格**

```json
{
    "status": 400,
    "msg": "未检测到人脸 / 有多张人脸",
    "result": {}
}
```

