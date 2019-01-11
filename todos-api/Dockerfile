FROM node:8-alpine

EXPOSE 8082

WORKDIR /usr/src/app

COPY package.json ./


RUN npm audit fix && npm install

COPY . .

CMD ["sh", "-c", "npm start" ]
