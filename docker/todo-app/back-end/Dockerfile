FROM node:14-alpine

WORKDIR /back-end

COPY package.json .
COPY package-lock.json .

RUN npm install

ADD node_modules.tar.gz .
COPY src ./src

EXPOSE 3001

ENTRYPOINT ["npm", "start"]