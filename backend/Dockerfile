# backend/Dockerfile
FROM node:20-alpine

WORKDIR /usr/src/app
COPY package*.json ./
RUN npm ci
COPY . .
EXPOSE 8888
CMD ["sh","-c","npm run setup && npm run dev"]

