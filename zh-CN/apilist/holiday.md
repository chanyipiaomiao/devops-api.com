---
name: 工作日节假日盘点
---

### API地址

```
GET https://devops-api.com/api/v1/holiworkday?date=2018-08-25

date: 要查询的日期 日期不足2位补0
```

返回:
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