FROM node:16-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

ARG ARG_NODE_PORT_DEFAULT=8080

ENV ARG_NODE_PORT=${ARG_NODE_PORT_DEFAULT}

EXPOSE $ARG_NODE_PORT

ENTRYPOINT [ "node" ]

CMD [ "server.js" ]