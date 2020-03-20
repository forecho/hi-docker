# 使用 [Docker Compose](https://docs.docker.com/compose/)

## 安装 

```
$ sudo curl -L https://get.daocloud.io/docker/compose/releases/download/1.25.4/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ docker-compose --version
```

## 后台（守护式）启动

```sh
$ sudo docker-compose up -d
```

然后通过 IP 可以访问 WordPress 程序。

## 查看容器信息

```sh
$ sudo docker-compose ps
```
