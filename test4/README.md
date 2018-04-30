# 实验4：图书管理系统顺序图绘制
|学号|班级|姓名|照片|
|:-------:|:-------------: | :----------:|:---:|
|201510414205|软件(本)15-2|黄伟|![flow1](../myself.jpg)|

### 1.1 查询图书用例
源码如下：

``` 
@startUml test4-1
title 图书查询
hide footbox
skinparam backgroundColor #ded
actor user
boundary 图书查询窗口
activate user
activate 图书查询窗口
user -> 图书查询窗口: 输入检索条件
图书查询窗口 -> 图书查询窗口: 验证输入信息
user -> 图书查询窗口: 点击查看详情
database book
图书查询窗口 -> book: 查询图书
activate book
book --> 图书查询窗口: 返回图书
@endUml
```
用例顺序图

![flow1](./test4-1.png)
### 1.2 预订图书用例
源码如下：
``` 
@startuml test4-2
actor user
user -> Book:查询书籍信息
user <-- Book:书籍信息
user -> BookRecord: 预定图书
user <-- BookRecord:预定结果
@enduml
```
用例顺序图

![flow1](./test4-2.png)
### 1.3 借阅图书用例
源码如下：
``` 
@startuml test4-3
actor manager
actor user
user -> manager:发起借阅请求
user <- manager:批准借阅
manager -> user:请求读者信息
manager <- user:得到读者信息
manager -> Book:请求书籍信息
manager <- Book:得到书籍信息
manager -> LendRecord:请求读者借阅信息
manager <- LendRecord:得到借阅信息
manager -> Book:减少书籍可借阅量
manager -> LendRecord:添加借阅记录
@enduml
```
用例顺序图

![flow1](./test4-3.png)