### 启动
```
cd server/compose
docker-compose up -d
```
docker stop $(docker ps -q) 停止所有容器

docker rm $(docker ps -aq) 删除所有容器

docker rmi $(docker images -q) 删除所有镜像

docker inspect myphp 查看容器配置信息
end

show master status
GRANT REPLICATION SLAVE ON *.* to 'backup'@'%' identified by 'backup';
show grants for 'backup'@'%';

CHANGE MASTER TO 
MASTER_HOST='192.168.10.126',
MASTER_PORT=3306,
MASTER_USER='backup',
MASTER_PASSWORD='backup';

START SLAVE;
show slave status;