#FROM node:19-alpine3.15
FROM node:18.15.0
WORKDIR /app
#COPY package.json .
COPY package*.json ./
RUN npm install
#COPY . .
COPY src ./src
EXPOSE 3000
#CMD ["node", "server.js"]
CMD ["node", "src/server.js"]