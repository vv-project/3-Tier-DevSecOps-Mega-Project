FROM node:22-alpine

WORKDIR /app
COPY package*.json ./
RUN npm ci
RUN  apk add --no-cache mysql-client
COPY . .
EXPOSE 5000
CMD ["node", "app.js"]

