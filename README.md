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