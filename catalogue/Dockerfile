FROM node:20
WORKDIR /app
COPY packege.json .
COPY server.js .
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node", "server.js"]