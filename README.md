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