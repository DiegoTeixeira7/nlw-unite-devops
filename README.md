# nlw-unite-devops

https://hub.docker.com/

docker build -t passin:v1 .
docker image ls
docker run -p 3001:3333 -d passin:v1
docker ps
docker ps -a
docker logs <id_container>
docker stop <id_container>
docker rm <id_container>

docker-compose up --build -d
docker-compose down
docker-compose up
