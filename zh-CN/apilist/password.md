---
name: 生成随机密码
---

### API地址

```
GET https://devops-api.com/api/v1/password/generation?name=root,user1,user2&specialChar=yes&length=48

length       指定长度 默认32位
name         指定多个名称，为多个名称生成密码
specialChar 是否添加特殊字符(!@#%$*.=)到密码里面 specialChar=yes 添加，其他不添加
```

返回:

```
{
    "data": {
        "password": {
            "root": "mU*zxN.vKljhh.L4Ulegvir7lUcEwJdhIenkjKZGhlDzEEN!",
            "user1": "TAmG*EaF.%J%Z$tJk=hNtcGH0AyKkFI.a7TUz5XrbXqZ0eHv",
            "user2": "2$sGahh5LV8J3evte2cEm6gjsZnX4cTrYnYYobu4lWaQwt!L"
        }
    },
    "entryType": "GenPassword",
    "errmsg": "",
    "requestId": "2cdd256e-d475-4e85-aa34-10f011f6fc9c",
    "statuscode": 0
}
```

也可以不添加任何参数,默认生成32位

```
GET https://devops-api.com/api/v1/password/generation
```