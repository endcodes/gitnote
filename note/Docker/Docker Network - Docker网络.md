# Docker  Network - Docker网络

## 查看docker网络列表

列出所有docker网络的网络名称

```shell
docker network ls
```

## 查看docker网络的详细信息


```shell
docker network inspect [网络名称]
```

## 新建docker网络

```shell
docker network create -d bridge [网络名称]
```

## 启动容器时指定docker网络

```shell
docker run -d --name [容器名称] --network [网络名称] [镜像名称]
```

参数：--network 用于指定容器的docker网络

### Host Network

```shell
docker run -d --name [容器名称] --network host [镜像名称]
```

参数--network制定为host时，容器和主机在同一网络命名空间中，容器中程序开启了端口，也会在主机中开启同样的端口。

## 将容器绑定到docker网络

```shell
docker network connect [网络名称] [容器名称]
```

##### 注意事项：

​	在自定义的docker网络中，各个容器之间可以直接使用容器名作为网络通信时的主机名（容器名与容器的IP地址等效）。默认的docker0网络不可以，需要使用--link参数。

