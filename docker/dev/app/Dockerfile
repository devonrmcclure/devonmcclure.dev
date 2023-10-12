# Dev build frontend
FROM node:20-alpine3.18 as app-dev

WORKDIR /app

COPY package*.json /app/
RUN npm ci

COPY . .
RUN npm run build
