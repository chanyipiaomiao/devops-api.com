---
name: IP地址归属地查询
---

### API地址

本功能使用了 [狮子的魂](https://gitee.com/lionsoul/ip2region) 项目提供的IP地址数据库

```
GET https://devops-api.com/api/v1/queryip?ip=IP地址
```

### 设置请求头部

头部名称:   DEVOPS-API-TOKEN

值: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoicHVibGljIiwidXBkYXRlVGltZSI6MTUzNTUzMzQ4NH0.JKxOjbtkmZC9FpPPkmF6u6AzBEYJt6m-yYyYr9wmx18

设置好请求头之后,就可以调用API了.

### 返回:

```
{
    "data": {
        "ip": "xxx.xxx.xxx.xxx",
        "ipInfo": {
            "CityId": 995,
            "Country": "中国",
            "Region": "0",
            "Province": "上海",
            "City": "上海市",
            "ISP": "电信"
        }
    },
    "entryType": "Query IP",
    "errmsg": "",
    "requestId": "6aae483e-5c72-4cb7-bbb7-50089e2da4d3",
    "statuscode": 0
}
```