# This is the official Node.js image from the Docker Hub
FROM node:14

# We will create and change to the app directory which is server here
WORKDIR /server

# here we will copy both package.json and package-lock.json
COPY package*.json ./

# This will help us to install app dependencies
RUN npm install

# copy source code of the server
COPY . .

# Expose port 3000
EXPOSE 3000

# Starting the server
CMD ["node", "server.js"]
