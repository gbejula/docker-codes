FROM node
WORKDIR /usr/app
RUN npm install -g nodemon
COPY package.json package.json
RUN npm install
RUN mv /usr/app/node_modules /node_modules
COPY . .
EXPOSE 80
CMD ["node", "server.js"]
