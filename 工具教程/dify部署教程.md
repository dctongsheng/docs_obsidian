
## 如何更新dify

```
git fetch origin
git checkout 1.0.0 # Switch to the 1.0.0 branch
cd docker
nano .env # Modify the environment configuration file to synchronizing .env.example file
docker compose -f docker-compose.yaml up -d


cd dify/docker
docker compose down
git pull origin main
docker compose pull
docker compose up -d
```
