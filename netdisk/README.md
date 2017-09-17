# 简介
大三上信息安全程序设计-安全加密网盘。
在一台机器上共享出一块安全的存储区域，其他计算机可从internet或wifi接入安全登录此存储空间，实现数据信息的安全存储和加密存储功能。

## 安装使用教程
客户端需安装配置tomcat，新建dynamic web project工程，在浏览器输入localhost:8080/slx访问主页进行登录注册。服务器端需安装mysql数据库并建好相应表。

## 模块简介
slx工程包括了前端文件和作为中转的servlet。netdisk工程包括了服务器端的socket监听和请求处理等。

## 具体实现
客户端的servlet，既作为BS的Server端接收前端页面的请求，同时作为CS的Client端向服务器转发请求并将响应返回给前端。加解密也由servlet实现。
