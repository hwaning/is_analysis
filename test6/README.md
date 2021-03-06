# 实验5：图书管理系统数据库设计与界面设计
## 成都大学信息科学与工程学院
|学号|班级|姓名|照片|
|:-------:|:-------------: | :----------:|:---:|
|201510414205|软件(本)15-2|黄伟|![flow1](../myself.jpg)|
## 1.概述
- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB
页面上。
- 学生的功能主要有：一是设置自己的GitHub用户名，二是查询自己的实验成绩。学生的GitHub用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。
## 2.系统总体结构
![flow1](./picture/总体设计.png)
页面设计[visist it](./InterfaceDesign/README.md)
## 3.用例图设计 [源码](./code/%E5%9F%BA%E4%BA%8EGitHub%E7%9A%84%E6%95%99%E5%8A%A1%E7%AE%A1%E7%90%86%E5%B9%B3%E5%8F%B0--%E7%94%A8%E4%BE%8B%E5%9B%BE.wsd)
![flow1](./picture/基于GitHub的教务管理平台--用例图.png)
## 4.类图设计 [源码](./code/类图.wsd)
![flow1](./picture/类图.png)
## 5.数据库设计 
### 数据库设计[visit it](./数据库设计.md)
## 6.用例及界面详细设计
- ### [“学生列表”用例](./case/学生列表.md)
- ### [“老师列表”用例](./case/老师列表.md)
- ### [“学期列表”用例](./case/学期列表.md)
- ### [“公告列表”用例](./case/公告列表.md)
- ### [“课程/实验/评分列表”用例](./case/课程列表用例.md)
- ### [“查看成绩”用例](./case/查看成绩用例.md)
- ### [“评定成绩”用例](./case/评定成绩用例.md)
- ### [“查看学生信息”用例](./case/查看用户信息用例.md)
- ### [“修改学生信息”用例](./case/修改用户信息用例.md)
- ### [“查看老师信息”用例](./case/查看用户信息用例.md)
- ### [“修改老师信息”用例](./case/修改用户信息用例.md)
- ### [“修改密码”用例](./case/修改密码用例.md)
- ### [“登录”用例](./case/登录用例.md)
- ### [“登出”用例](./case/登出用例.md)
