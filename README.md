## Available Scripts

In the project directory, you can run:

### Build with docker (dev)
docker build -f .\Dockerfile.dev .

### Run with docker
docker run -it -p 3000:3000 -e CHOKIDAR_USEPOLLING=true -v /app/node_modules -v ${pwd}:/app CONTAINER_ID

### Run with docker compose
docker-compose up