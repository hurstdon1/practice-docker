FROM node:16-alpine AS builder

WORKDIR /ng-app

RUN apk update
RUN apk add --no-cache git

COPY package*.json .
RUN npm install
COPY . .

CMD ["npm", "start"]