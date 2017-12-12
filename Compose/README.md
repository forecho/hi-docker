# 使用 [Docker Compose](https://docs.docker.com/compose/)

## 安装 

```
$ sudo curl -L https://get.daocloud.io/docker/compose/releases/download/1.17.1/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ docker-compose --version
```

```sh
$ sudo docker-compose up -d
$ sudo docker-compose ps
```

然后通过 IP 可以访问 WordPress 程序。