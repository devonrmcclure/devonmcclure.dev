# Prod build
FROM node:20-alpine3.18 as app-prod

ARG user=devon-portfolio
ARG uid=2200
RUN adduser -u $uid -D $user

WORKDIR /app

COPY package*.json /app/
RUN npm ci --omit dev

COPY . .
RUN npm run build

RUN chown -R $user:$user /app

USER $user

