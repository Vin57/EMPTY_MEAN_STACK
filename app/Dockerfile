FROM node:16.13.2-slim as node
### ANGULAR ###
WORKDIR /usr/app

COPY package*.json ./

RUN npm install

EXPOSE 4200 49153

COPY . .

RUN npm run build

CMD [ "npm", "start"]
