# syntax=docker/dockerfile:1

FROM node:8

ENV NODE_ENV=production

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install --production

COPY . .

EXPOSE 4040

CMD [ "node", "server.js" ]