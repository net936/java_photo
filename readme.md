
## 项目简介


>该项目是基于Java+Springboot+Vue开发的在线摄影预约管理系统（前后端分离），这是一项为大学生课程设计作业而开发的项目。
该系统旨在帮助大学生学习并掌握Java编程技能，同时锻炼他们的项目设计与开发能力。通过学习基于Java的在线摄影管理系统项目，大学生可以在实践中学习和提升自己的能力，为以后的职业发展打下坚实基础。如需完整源码，可以联系客服微信购买：lengqin1024


## 在线演示

演示地址：[https://photo.gitapp.cn](https://photo.gitapp.cn)





## 主要功能

- 套餐管理：管理系统可以录入、修改和查询套餐的基本信息，如名称、价格、备注等。
- 类型管理：系统可以管理套餐的类型信息，包括类型的名称等。
- 评论管理：管理和浏览整个网站的评论信息。
- 用户管理：管理和浏览网站的用户信息，可以新增、编辑和删除用户。
- 统计分析：系统可以根据套餐的活动数据和用户参与度进行统计和分析，帮助管理员了解整个系统的状况。
- 消息管理：套餐管理员可以在系统上发布消息，整个网站的用户都能收到。
- 广告管理：套餐管理员可以在系统上发布广告消息，然后在详情页面右侧展示。
- 意见反馈：套餐管理员可以在后台查看浏览用户提交的意见反馈信息。
- 系统信息：管理员可以查看系统的基本信息，包括系统名称、服务器信息、内存信息、cpu信息、软件信息等。
- 注册登录：用户通过注册和登录后，才能使用网站。
- 门户浏览：用户进入首页后，可以浏览套餐列表信息，包括最新、最热。
- 热门推荐：基于协同过滤推荐算法的热门推荐。
- 用户中心：包括用户基本资料修改、用户基本信息、密码、收藏点赞等。
- 我的预约：包括我预约的套餐的信息。
- 意见反馈：包括用户提交意见反馈的入口页面。
- 模糊搜索：顶部搜索功能，支持模糊搜索套餐信息。
- 套餐评论：详情页下侧用户可以评论套餐。

## 开发环境

- 后端： Java 8 + Springboot
- 前端： Javascript + Vue
- 数据库：MySQL 5.7
- 开发平台：IDEA + vscode
- 运行环境：Windows 10/11

## 关键技术

- 前端技术栈 ES6、vue、vuex、vue-router、vue-cli、axios、antd
- 后端技术栈 Java、Springboot、mybatis



## 运行步骤

### 软件准备

1. IDEA 2022 [下载地址](https://download.jetbrains.com/idea/ideaIU-2022.3.3.exe)
2. MySQL 5.7 [下载地址](https://dev.mysql.com/get/Downloads/MySQLInstaller/mysql-installer-community-5.7.44.0.msi)
3. Node [下载地址](https://nodejs.org/dist/v18.20.2/node-v18.20.2-x64.msi)


### 后端运行步骤

(1) 使用IDEA打开server目录，设置项目的jdk，同步maven依赖。

(2) 创建数据库，创建SQL如下：
```
CREATE DATABASE IF NOT EXISTS java_db[your dbname] DEFAULT CHARSET utf8 COLLATE utf8_general_ci
```
(3) 恢复数据库数据。在mysql下依次执行如下命令：

```
mysql> use xxx(数据库名);
mysql> source D:/xxx/xxx/xxx.sql;
```

(4) 配置数据库。在application.yml中配置您的数据库账号密码

```
DB_NAME: [db_name]
spring:
  datasource:
    username: root
    password: [your password]
    url: jdbc:mysql://localhost:3306/${DB_NAME}?useUnicode=true&characterEncoding=utf-8&useSSL=true&serverTimezone=UTC
    driver-class-name: com.mysql.cj.jdbc.Driver
    type: com.alibaba.druid.pool.DruidDataSource
```

(5) 启动服务。点击IDEA的运行按钮。


### 前端运行步骤

(1) 安装依赖，cd到web目录，执行:
```
npm install 
```
(2) 运行项目
```
npm run dev
```

然后访问前端地址。即可


## 开发文档

[点击进入](doc/doc.md)


## 付费咨询

微信（Lengqin1024）

## 常见问题

**1. 数据库版本有什么要求？**

答：mysql 5.7及以上版本即可

**2. 项目的代码结构？**

答：server目录是后端代码，web目录是前端代码。

**3. 需要学习哪些技术知识？**

答：需要学习[Java编程知识](https://www.w3cschool.cn/java/)、[springboot框架知识](https://springdoc.cn/spring-boot/)、[vue编程知识](https://cn.vuejs.org/guide/introduction.html)

**4. 后台管理的默认账号密码是？**

答：管理员账号密码是：admin123 / admin123

**5. 后台管理提示演示账号权限不足 怎么办？**

答： 将演示账号变为管理员即可。修改role为3.

