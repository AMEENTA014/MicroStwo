FROM node:20-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm ci --omit=dev

COPY src/ .

EXPOSE 4000

CMD ["node", "server.mjs"]
