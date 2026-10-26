FROM node:20
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV Environment=REDIS_HOST=redis \
    Environment=CATALOGUE_HOST=catalogue \
    Environment=catalogue=8080
CMD ["node", "server.js"]