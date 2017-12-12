# hi-docker

此项目是学习 docker 的示例代码仓库，实例主要来自于 《Docker 经典实例》 这本书

## 安装 Docker

```sh
$ sudo curl -sSL https://get.daocloud.io/docker | sh
```

**换国内源**

```sh
$ sudo curl -sSL https://get.daocloud.io/daotools/set_mirror.sh | sh -s http://d52bcda9.m.daocloud.io
```

## 基本使用

**安装镜像**

```sh
$ sudo docker run fedora cat /etc/os-release
```

**查看镜像**

```sh
$ sudo docker images
```

**查看当前容器**

```sh
$ sudo docker ps
```

**启动容器的交互界面**

```sh
$ sudo docker -it fedora /bin/bash
```


**把容器保存为镜像**

```sh
$ sudo docker ps -a
$ sudo docker commit [容器ID] [名称]
$ sudo docker images
```


**删除容器**

```sh
$ sudo docker ps -a | grep <container-id>
$ sudo docker stop <container-id>
$ sudo docker rm <container-id>
$ sudo docker rmi <image-id>
```

**进入容器环境/启动容器的交互界面**

```sh
$ sudo docker exec -ti [容器 ID/容器 Name] /bin/bash
```

**删除所有停止中的容器**

```sh
$ sudo docker rm $(sudo docker ps -a -q)
```

## 参考资料

- [Docker 极速下载](http://get.daocloud.io/)
- [《Docker 经典实例》书中代码](https://github.com/how2dock/docbook)