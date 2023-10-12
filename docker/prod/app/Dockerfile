# Dev build frontend
FROM node:20-alpine3.18 as app-prod

WORKDIR /app

COPY package*.json /app/
RUN npm ci --omit dev

COPY . .
RUN npm run build
