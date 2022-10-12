FROM mjgargani/puppeteer:trybe1.0

WORKDIR /tests

COPY package.json .
COPY package-lock.json .

RUN npm install

ADD node_modules.tar.gz .
COPY jest.config.js .
COPY e2e ./e2e

ENTRYPOINT ["npm", "test"]