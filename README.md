# fc4-docker-for-development
|Commands|
|-|
| docker build -t brunorodrigoss/mynodeimage:latest -f Dockerfile.dev . --no-cache |
||
| chown brunorodrigo:brunorodrigo test.txt |
| ls -la . |
| whoami |
| cat /etc/passwd |
||
| docker run -v $(pwd):/home/node/app -it brunorodrigoss/mynodeimage:latest bash |
| npm init |
||
| chmod +x start.sh |
||
| docker compose -f docker-compose.dev.yaml up |
| docker compose -f docker-compose.dev.yaml exec web bash |
| docker compose -f docker-compose.dev.yaml up --build |
| npm install express mysql2|
| node src/index.js |
| npm start |
||
| docker compose -f docker-compose.dev.yaml exec db bash |
| printenv |
| nodemon src/index.js |
| NODEMON_VERSION=3.1.5 docker compose -f docker-compose.dev.yaml up --build |
||
| docker compose -f docker-compose.dev.yaml ps |
| docker network ls |
||
| docker compose -f docker-compose.test.yaml up |
||
| docker compose -f docker-compose.dev.yaml --profile debug up |
| docker compose -f docker-compose.dev.yaml --profile nginx up |
| docker compose -f docker-compose.dev.yaml --profile nginx --profile debug up |
||
| docker compose -f docker-compose.watch.yaml --profile nginx up --watch |
| docker compose -f docker-compose.watch.yaml --profile nginx logs nginx |
| docker compose -f docker-compose.watch.yaml exec nginx sh |
| cat /etc/nginx/nginx.conf |
||
| export COMPOSE_FILE=docker-compose.dev.yaml:docker-compose.override.yaml |
| docker compose config |
| docker compose up |
| docker compose -f docker-compose.dev.yaml -p feature-xpto up |
| export COMPOSE_PROJECT_NAME=feature-xpto |
| docker compose -f docker-compose.dev.yaml up |
| docker compose -f docker-compose.dev.yaml -p feature-xpto ps |