# 获得用户信息



得到自己的全面信息



### HTTP

> GET /get_user



### 参数

不需要，有 cookie 行



### 返回



成功的返回

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
      "status": 200,
      "msg": "OK",
      "result": {
        "name": "刘思宁",
        "avatar_url": "",
        "mixin_id": 37230353,
        "description": "",
        "has_image": false,
        "image": "",
        "beauty": 0,
        "gender": "",
        "age": 0,
        "display_image": false,
        "rank": 14,
        "income": 0.1,
        "tip_transations": {
          "count": 5,
          "to_boy": 2,
          "to_girl": 3,
          "images": [
            "https://s3-ap-northeast-1.amazonaws.com/wohaokan.me/hahahaha.jpeg",
            "https://s3-ap-northeast-1.amazonaws.com/wohaokan.me/hahahaha.jpeg",
            "https://s3-ap-northeast-1.amazonaws.com/wohaokan.me/hahahaha.jpeg",
            "https://s3-ap-northeast-1.amazonaws.com/wohaokan.me/hahahaha.jpeg",
            "https://s3-ap-northeast-1.amazonaws.com/wohaokan.me/hahahaha.jpeg"
          ]
        }
      }
    }
}
```



说明：

1. has_image 表示用户是否有照片
2. display_image 表示用户是否**上架**自己的照片