# root/server/Dockerfile
FROM node:24-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

# Copy the rest of the server source
COPY . .

EXPOSE 1234

CMD ["npm", "start"]

# docker run -d --env-file .env -p 1234:1234 dating-site-server
