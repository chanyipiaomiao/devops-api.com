---
name: 获取字符串的MD5值
---

### API地址

```
GET https://devops-api.com/api/v1/md5?rawstr=123456

rawstr: 原始字符串
```

### 设置请求头部

头部名称:   DEVOPS-API-TOKEN

值: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoicHVibGljIiwidXBkYXRlVGltZSI6MTUzNTUzMzQ4NH0.JKxOjbtkmZC9FpPPkmF6u6AzBEYJt6m-yYyYr9wmx18

设置好请求头之后,就可以调用API了.

### 返回:

```
{
    "data": {
        "rawString": "123456",
        "rawStringMD5": "e10adc3949ba59abbe56e057f20f883e"
    },
    "entryType": "Get String MD5",
    "errmsg": "",
    "requestId": "3d3f0828-c0e2-47a6-b54d-4e00f16ee2eb",
    "statuscode": 0
}
```