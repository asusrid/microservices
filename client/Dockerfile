FROM node:alpine

# to solve current bug with create-react-app with docker containers

WORKDIR /app

COPY ./package.json ./
RUN npm install
COPY ./ ./

CMD [ "npm", "start" ]