# metasploit-POC
>github repository

* 實習期間所撰寫的 metasploit exploit module
    1. 環境建置 & cve-2020-14882
    2. cve-2021-41277
    3. cve-2022-29464
    4. cve-2022-26352

* docker 常用命令: [取自這裡](https://kknews.cc/code/kp2yv8p.html)
```shell=1
Docker的常用命令
#系統命令
systemctl start docker                          #啟動docker
systemctl stop docker                           #停止docker
systemctl restart docker                        #重啟docker
systemctl enable docker                         #設置docker開機自啟
#基本命令
docker version                                          #查看docker版本
docker info                                                     #查看docker詳細信息
docker --help                                           #查看docker命令
#鏡像命令
docker images                                           #查看docker鏡像列表
docker images -a                                        #列出本地所有鏡像
docker images --digests                         #顯示鏡像的摘要信息
docker search redis                                     #從Docker Hub上查找redis鏡像
docker pull redis                                       #從Docker Hub上下載redis鏡像
docker rmi 373f0984b070                         #刪除IMAGE ID 為373f0984b070的鏡像
#運行命令
#-p 6379:6379   埠映射：前表示主機部分,後表示容器部分
#-d     在後台運行容器（不進入終端）並列印容器ID/容器名
#--name myredis表示自定義容器名為myredis
docker run -d -p 6379:6379 --name myredis redis:latest          #根據鏡像創建並運行容器
#容器命令
docker container ls 或 docker ps                         #查看正在運行的容器
docker container ls -a 或 docker ps -a                   #列出所有容器
docker container start 容器ID 或 容器名稱              #啟動容器
docker start 容器ID 或 容器名稱                                        #啟動容器
docker container stop 容器ID 或 容器名稱                       #停止容器
docker stop 容器ID 或 容器名稱                                 #停止容器
docker container rm 容器ID 或 容器名稱                 #刪除容器
docker rm 容器ID 或 容器名稱                                           #刪除容器
docker container logs -f 容器ID 或 容器名稱            #查看容器日誌
docker exec -it name /bin/bash                                  #進入name（容器名/id）中開啟交互式的終端，exit退出
```
