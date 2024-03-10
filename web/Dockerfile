#FROM node:19-alpine3.15
FROM node:18.15.0
WORKDIR /app
COPY package.json .
RUN npm install
RUN mkdir -p node_modules/.cache && chmod -R 777 node_modules/.cache
COPY . .
EXPOSE 3000
CMD ["npm", "run", "start"]