# 一、运行容器
docker run --name myubuntu -it

-it :以交互命令
-p 8082:8080 :把docker中的8080端口映射到宿主机的8082端口
-name :自定义名称

# 二、退出容器
- 退出不停止容器 <ctrl+p+q>
- exit 退出当前连接docker客户端(假如只有一个客户端直接会停止容器)


# 三 再次进入容器
docker exec -it myubuntu /bin/bash

# docker

# 复制文件到宿主机
- docker cp  myubuntu:/opt/hello.log  ./
- docker cp  ./hi.log  myubuntu:/opt/
