### How to run docker file in terminal

docker build -f Dockerfile.dev .

### How to run dock and browser updates any changes in html in terminal
### (ONLY works for mac)

docker run -p 3000:3000 -v /app/node_modules -v$(pwd):/app <imageId>

### Run test

docker run -it <imageId> npm run test

## if server running, to run test and changes are automatic

docker exec -it <imageId> npm run test

### Build the image with all changes including test
###(Add --build tag if make any changes:docker-c... -- build)
docker-compose up

### Stop the containers

docker-compose down
