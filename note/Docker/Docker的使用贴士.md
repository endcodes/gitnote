# Docker的使用贴士

## 在docker中启动mysql

```shell
sudo docker run -d --name=[容器名称] -p [主机上的端口]:3306 -e MYSQL_ROOT_PASSWORD=[root密码] -v [主机上卷存储地址]:/var/lib/mysql mysql
```


