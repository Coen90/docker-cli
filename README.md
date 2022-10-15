# docker-cli

docker network ls
docker network create redis-net

docker run --name my-redis -p 6379:6379 --network redis-net -d redis redis-server --appendonly yes
