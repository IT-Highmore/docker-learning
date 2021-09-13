# docker-learning

## 拉取镜像
docker pull ${image}
## 推送镜像
docker push ${image}
## 镜像打标签
docker tag ${image_id} ${tag_name}
## 查看当前所有正在运行的容器
docker ps
## 查看当前停止和运行的容器
docker ps -a
## 查看当前容器的日志
docker logs -f ${container_id}
## 进入容器命令
docker exec -it ${container_id} /bin/sh 
## 运行容器命令
docker run ...
## 容器停止
docker stop ${container_id}
## 容器重启
docker restart ${container_id}
## 青云容器登录
echo $(IMAGE_REPO_PASS) | docker login -u $(IMAGE_REPO_USER) --password-stdin dockerhub.qingcloud.com
## 查看当前挂载
docker volume ls
## 创建挂载
docker volume create ${volume}
## 删除挂载
docker volume rm ${volume}
## 查看当前网络
docker network ls
## 创建网络
docker network create ${net_name}
## 删除网络
docker network rm ${net_name}

## 查看当前的运行的docker
docker-compose ps
## 后台运行
docker-compose up  -d
## 启动某个容器
docker-compose up  ${docker-compose-name}
## 关闭与删除
docker-compose stop && docker-compose down

