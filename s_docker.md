# 下载

# 命令
## 下载镜像
- docker search
- docker pull
- docker images
- docker rmi

## 启动容器
- docker run
```sh
//-d后台运行 本机88端口映射到容器80端口
docker run -d --name mynginx -p 88:80 nginx
```
- docker ps
- docker stop
- docker start
- docker restart
- docker stats
- docker logs
- docker exec
```sh
//进入到容器mynginx
docker exec -it mynginx /bin/bash
```
- docker rm

## 保存镜像
- docker commit
```sh
docker commit -m "update" mynginx mynginx:v1.0
```
- docker save
```sh
docker save -o mynginx.tar mynginx:v1.0
```
- docker load
```sh
docker load -i mynginx.tar
```

## 分享镜像
- docker login
- docker tag
- docker push
