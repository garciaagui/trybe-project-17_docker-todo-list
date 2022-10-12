FROM node:14-alpine

WORKDIR /front-end

COPY package.json .
COPY package-lock.json .
RUN npm install

ADD node_modules.tar.gz .
COPY src ./src
COPY public ./public

EXPOSE 3000

ENTRYPOINT ["npm", "start"]