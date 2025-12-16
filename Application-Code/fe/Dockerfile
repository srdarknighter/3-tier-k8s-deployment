FROM node:18-alpine
WORKDIR /app

ENV NODE_OPTIONS=--openssl-legacy-provider

COPY package*.json ./
RUN npm ci

COPY . .
CMD ["npm", "start"]
