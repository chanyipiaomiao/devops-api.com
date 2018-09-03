---
name: 工作日节假日判断
---

### API地址

```
GET https://devops-api.com/api/v1/holiworkday?date=2018-08-25

date: 要查询的日期 日期不足2位补0
```

### 设置请求头部

头部名称:   DEVOPS-API-TOKEN

值: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoicHVibGljIiwidXBkYXRlVGltZSI6MTUzNTUzMzQ4NH0.JKxOjbtkmZC9FpPPkmF6u6AzBEYJt6m-yYyYr9wmx18

设置好请求头之后,就可以调用API了.

### 返回:
```
{
    "data": {
        "date": "2018-08-25",
        "dateType": "weekend"
    },
    "entryType": "Get Holiday/Workday",
    "errmsg": "",
    "requestId": "562444c2-1a48-4c69-9ed1-d2553dea3cba",
    "statuscode": 0
}

dateType: 有3种 workday: 工作日  holiday: 节假日  weekend: 周末
```