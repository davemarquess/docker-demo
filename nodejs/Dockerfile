# https://nodejs.org/en/docs/guides/nodejs-docker-webapp/

# LTS // confidence that this version of node will be supported for 5 years
#starting point, where the image is coming from
# FROM node:10.13.0

# Latest
FROM node:latest

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm install --only=production

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "npm", "start" ]
