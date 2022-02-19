<!-- LAB 2 -->
<!-- Docker build -->
build -t usermgmt:latest .

<!-- Docker run -->
docker run -d --name User -p 3000:3000 usermgmt:latest

<!-- URL -->
localhost:3000


<!-- LAB 3 -->
<!-- deploy the stack  -->
docker stack deploy -c docker-compose.yaml myapp-stack

<!-- scaling out first service -->
docker service scale myapp-stack_service1=7

<!-- scaling in first service -->
docker service scale myapp-stack_service1=2

<!-- remove stack -->
docker stack rm myapp-stack