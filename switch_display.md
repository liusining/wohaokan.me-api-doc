# 上架 / 下架自己的图片



展示 或 不展示自己的图片



###  HTTP



> POST /switch_display



### 参数

不需要



### 返回



成功的返回

```json
{
    "status": 200,
    "msg": "OK",
    "result": {
        "display_image": false
    }
}
```

会返回最新的状态