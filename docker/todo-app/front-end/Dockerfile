FROM node:14-alpine

WORKDIR /app

EXPOSE 3000

ADD node_modules.tar.gz ./
COPY package.json ./
COPY package-lock.json ./
COPY src ./src

RUN npm install

ENTRYPOINT ["npm", "start"]
