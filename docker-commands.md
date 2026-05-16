🐳 Docker Commands Cheat Sheet
1. Images
docker pull <image> → Download image from Docker Hub

docker images → List all images

docker rmi <image> → Remove image

2. Containers
docker run -it <image> bash → Run container interactively

docker ps → List running containers

docker ps -a → List all containers (including stopped)

docker stop <id> → Stop container

docker rm <id> → Remove container

3. Build
docker build -t <name> . → Build image from Dockerfile

docker exec -it <id> bash → Run command inside container

docker logs <id> → Show container logs

4. Networking
docker run -p 8080:80 nginx → Map host port 8080 → container port 80

docker inspect <id> → Show container details

5. Volumes
docker run -v $(pwd):/app ubuntu ls /app → Mount host folder

docker volume create mydata → Create named volume

docker run -v mydata:/data ubuntu → Use persistent volume

6. Docker Compose
docker-compose up --build → Start services

docker-compose down → Stop services

docker-compose ps → List services