docker stack deploy -c docker-compose.yaml dockerlab2-stack
docker stack services dockerlab2-stack
docker service scale dockerlab2-stack_mywebsite=7
docker stack services dockerlab2-stack
docker service scale dockerlab2-stack_mywebsite=2
docker stack services dockerlab2-stack
docker stack rm dockerlab2-stack
docker rm 8c46f0b3607511ba11fdf7b6e9641daca9bf643164a7a86b1b56a0875e375f98