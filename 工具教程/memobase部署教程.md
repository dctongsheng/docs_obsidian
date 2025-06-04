先部署[[redis部署教程]]然后部署[[postsql部署教程]]

编写配置文件
```
DATABASE_URL=DATABASE_URL=postgresql://postgres:mysecretpassword@192.168.0.119:54332/memobase
REDIS_URL=redis://:helloworld@localhost:6379
ACCESS_TOKEN=secret

PROJECT_ID=memobase_dev
```

# 基于docker compose安装

