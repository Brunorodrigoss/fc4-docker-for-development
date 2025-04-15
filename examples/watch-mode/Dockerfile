FROM node:22.8.0-slim

RUN apt update &&  apt install -y procps

USER node

RUN mkdir -p /home/node/app

WORKDIR /home/node/app

COPY --chown=node:node package*.json .
RUN npm install

COPY --chown=node:node . .

EXPOSE 3000

CMD [ "tail", "-f", "/dev/null" ]