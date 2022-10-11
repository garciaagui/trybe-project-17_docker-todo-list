FROM mjgargani/puppeteer:trybe1.0

WORKDIR /app

ADD node_modules.tar.gz ./
COPY package.json ./
COPY package-lock.json ./
COPY jest.config.js ./
COPY e2e ./e2e

RUN npm install

ENTRYPOINT ["npm", "test"]
