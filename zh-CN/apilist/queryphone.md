---
name: 手机归属地查询
---

### API地址

本功能使用了 [xluohome](https://github.com/xluohome/phonedata) 项目提供的手机归属地数据库


```
GET https://devops-api.com/api/v1/queryphone?phone=手机号

phone: 要查询的手机号
```

### 设置请求头部

头部名称:   DEVOPS-API-TOKEN

值: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoicHVibGljIiwidXBkYXRlVGltZSI6MTUzNTUzMzQ4NH0.JKxOjbtkmZC9FpPPkmF6u6AzBEYJt6m-yYyYr9wmx18

设置好请求头之后,就可以调用API了.

### 返回:

```
{
    "data": {
        "AreaZone": "021",
        "CardType": "中国移动",
        "City": "上海",
        "PhoneNum": "xxxxxxxxxx",
        "Province": "上海",
        "ZipCode": "200000"
    },
    "entryType": "Query Phone Location",
    "errmsg": "",
    "requestId": "0860edaa-db7f-46ee-ac89-d41eeb2ed80d",
    "statuscode": 0
}
```
