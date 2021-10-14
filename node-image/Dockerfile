# Specify base image
FROM node:alpine

# Working directory inside the file system of the container
WORKDIR /usr/app

# copy this first to make sure modules dont get reinstalled every time code changes
COPY ./package.json ./

# install dependencies
RUN npm install

# copy all files and folders into the container
COPY ./ ./

# default command
CMD ["npm", "start"]