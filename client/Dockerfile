FROM node:alpine

# to solve current bug with create-react-app with docker containers
ENV CI = true
ENV WDS_SOCKET_PORT = 0

WORKDIR /app

COPY ./package.json ./
RUN npm install
COPY ./ ./

CMD [ "npm", "start" ]