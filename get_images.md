# 展示一张照片



获得一张照片的 URL。



### HTTP

> GET /get_images?page=<page-number>



### 参数

| 名称 | 类型      | 必须？ | 默认值 | 说明                     |
| ---- | --------- | ------ | ------ | ------------------------ |
| page | url param | 否     | 1      | 页面，防止返回重复的图片 |



### 返回

**如果未登录**

只返回一张固定的图片

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "images": [
            {
                "url": "https://example.com/abc.jpg",
                "likes": 17
            }
        ]
    }
}
```



**如果已登录**

返回 10 张照片

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "images": [
            {
                "url": "https://example.com/abc.jpg",
                "likes": 17
            },
            {
                "url": "https://example.com/abc.jpg",
                "likes": 17
            },
            {
                "url": "https://example.com/abc.jpg",
                "likes": 17
            }
        ]
    }
}
```

