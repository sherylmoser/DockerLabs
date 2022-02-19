<!-- Docker build -->
build -t usermgmt:latest .

<!-- Docker run -->
docker run -d --name User -p 3000:3000 usermgmt:latest

<!-- URL -->
localhost:3000