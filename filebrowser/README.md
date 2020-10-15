# docker-compose
fb 文件浏览器 详情访问 https://hub.docker.com/r/80x86/filebrowser
unraid 用户安装 docker-compose 方法，来自https://forums.unraid.net/topic/91436-is-docker-compose-available-on-unraid/
命令行输入下面两行：
```
curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```
安装完毕
根据自己的配置，将本文件拷贝到合适的目录下，并命令行进入此目录，然后执行：
```
docker-compose up -d
```
之后访问unraid ip:8082 即可
如果想停止容器，可以输入以下命令
```
docker-compose stop  #停止容器
```
如果想更新容器，可以先停止容器，修改配置，再启动容器
```
docker-compose stop 
...#修改配置
docker-compose up -d
```

想了解docker-compose 的可以访问 https://docs.docker.com/compose/compose-file/
