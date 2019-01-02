# wohaokan.me backend API



## 环境

测试环境： stg.api.wohaokan.me

生产环境：api.wohaokan.me



## 状态码

除非授权失败（比如未登录），或服务器异常，否则服务器均返回 http 200。

response body 中自带一套 status 码：

1. 200 为成功
2. 400 为不成功

如果 session-key 失效，怎返回： 

http 200 ，body 为：

```json
{
  "status": 700,
  "msg": "invalid session key",
  "result": {}
}
```



## 验证机制

在需要验证用户的 requests 中加入一个 header： `X-Session-Key`



各接口文档，见各文件。
