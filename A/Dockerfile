FROM node:alpine

RUN apk update && \
  apk add \
   nano \
   mongodb \
   nodejs && \
   mkdir /app \
   mkdir /src

WORKDIR /src
ADD app.js app.js
ADD package.json package.json
ADD package-lock.json package-lock.json
RUN npm install

COPY . .
