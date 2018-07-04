FROM node:8-alpine as base
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .

FROM base
EXPOSE 3000
USER node

CMD ["npm", "start"]
