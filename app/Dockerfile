FROM node:alpine
WORKDIR /usr/app
COPY package.json .
RUN npm install --quiet
COPY . .
EXPOSE 8081
CMD [ "npm", "run", "start" ]