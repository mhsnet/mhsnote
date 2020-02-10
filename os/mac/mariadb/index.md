# [《MHS笔记》] > [《mariadb使用》]

## 安装
```
# 查询
$ brew search mariadb
# 安装
$ brew install mariadb
# 运行数据库安装程序
$ mysql_install_db
# 启动服务
$ mysql.server start
# 安全的完成安装(pw123456)
$ mysql_secure_installation
# 开机启动（$ brew services -h）
$ brew services start mariadb
# 连接
$ mysql -u root -p
```

## mysql 基本使用
```
# 查看字符集
> show variables like '%character%';
# 显示数据库
> show databases;
# 创建数据库(mhstest)
> create database mhstest;
# 删除数据库(mhstest)
> drop database mhstest;
# 使用数据库(mhstest)
> use mhstest;
# 显示数据表
> show tables;
# 删除表(test_user)
> drop table test_urer;
# 显示表结构(test_user)
> desc test_user;
# 显示表记录(test_user)
> select * from test_user;
# 清空表记录(test_user)
```

## 
[《MHS笔记》]: https://mhsnet.github.io/mhsnote/ "《MHS笔记》"

[《mariadb使用》]: https://mhsnet.github.io/mhsnote/os/mac/mariadb/index.html "《mariadb使用》"