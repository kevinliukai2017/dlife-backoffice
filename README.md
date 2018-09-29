# dlife-backoffice
dLife aims to build an online family for all Digital people

dLife backoffice is management tool to manage all activities created from dLife, and also it could be a fundation of backoffice management capability for the team instead of creating everything from scratch.

Based on open source project Bootdo, which also based on Sprint Boot, MyBatis, Shiro, Ehche etc..

技术选型

1、后端
核心框架：Spring Boot
安全框架：Apache Shiro
模板引擎：Thymeleaf
持久层框架：MyBatis
数据库连接池：Alibaba Druid
缓存框架：Ehcache 、Redis
日志管理：SLF4J
工具类：Apache Commons、Jackson
2、前端

JS框架：jQuery
客户端验证：JQuery Validation
富文本在线编辑：summernote
数据表格：bootstrapTable
弹出层：layer
树结构控件：jsTree
4、平台

服务器中间件：SpringBoot内置
数据库支持：目前仅提供MySql数据库的支持，但不限于数据库
开发环境：Java、Eclipse Java EE 、Maven 、Git
安全考虑

开发语言：系统采用Java 语言开发，具有卓越的通用性、高效性、平台移植性和安全性。
分层设计：（数据库层，数据访问层，业务逻辑层，展示层）层次清楚，低耦合，各层必须通过接口才能接入并进行参数校验（如：在展示层不可直接操作数据库），保证数据操作的安全。
双重验证：用户表单提交双验证：包括服务器端验证及客户端验证，防止用户通过浏览器恶意修改（如不可写文本域、隐藏变量篡改、上传非法文件等），跳过客户端验证操作数据库。
安全编码：用户表单提交所有数据，在服务器端都进行安全编码，防止用户提交非法脚本及SQL注入获取敏感数据等，确保数据安全。
密码加密：登录用户密码进行SHA1散列加密，此加密方法是不可逆的。保证密文泄露后的安全问题。
强制访问：系统对所有管理端链接都进行用户身份权限验证，防止用户直接填写url进行访问。
