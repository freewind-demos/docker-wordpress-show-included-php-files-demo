Docker Wordpress MySql Demo
===========================

通过docker-compose将多个docker images（wordpress, mysql, phpMyAdmin) 组合起来，
搭建一个本地的快速开发wordpress环境。

本地`WordPress-5.3.2`中的文件将被映射到docker container里，我们的修改刷新浏览器后马上可以看到效果。

`docker-entrypoint-initdb.d`下是sql的初始化文件，启动时会自动使用它来初始化数据库

```
npm run up
```

当前登录wordpress的用户名和密码是：

```
freewind
123456
```

