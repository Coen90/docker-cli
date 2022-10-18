# docker-cli

docker network ls
docker network create redis-net

docker run --name my-redis -p 6379:6379 --network redis-net -d redis redis-server --appendonly yes

docker run -d --name mariadb -e MYSQL_DATABASE=prod -e MYSQL_USER=user01 -e MYSQL_PASSWORD=user01 -e MYSQL_ROOT_PASSWORD=password -p 33306:33306 /app/maria:/var/lib/mysql mariadb
