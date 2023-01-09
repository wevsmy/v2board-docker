# 使用 Docker 安装 V2Board

### 安装 Docker
```
curl -fsSL https://get.docker.com | bash
curl -L "https://github.com/docker/compose/releases/download/1.25.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod a+x /usr/local/bin/docker-compose
```

### 克隆代码
```
git clone https://github.com/wevsmy/v2board-docker.git
cd v2board-docker/
git submodule update --init
git submodule update --remote
```

### 启动环境

```
docker-compose up -d
```

### 安装配置 V2Board
```
docker-compose exec v2board bash
bash-5.0# bash init.sh
数据库地址： mysql
数据库名：v2board
数据库用户名：root
数据库密码：v2boardisbest
```