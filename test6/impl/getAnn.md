#### 用例： 课程列表
- 权限： 无需权限
- 功能： 返回所有公告的列表。
- API请求地址： 接口基本地址/api/getAnn
- 请求方式 ： GET
- 请求参数说明: 无
```
 {
      "status": true,
      "info": "获取结果成功",
      "total": 36,
      "data": [
          {
          "ID":19,
          "ANN_NO":"41052",
          "TITLE":"****",
          "CONTENT": "内容",
          "STATUS":"1",
          "ADDTIME": "2018-05-22 17:48:01",
          ...
          },
          
          {
          ...其他课程
          }
      ]
  }

```
- 返回参数说明：

参数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
total |返回公告数量
ID | 	数据库自增
title |公告标题
content | 公告内容
STATUS |是否正常
ADDTIME | 增加日期

