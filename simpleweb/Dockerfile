# Specify a base image
FROM node:14-alpine

WORKDIR /usr/app

# Move package.json as it's own step for caching
COPY ./package.json ./

# Install some dependencies
RUN npm install

COPY ./ ./

# Default command
CMD ["npm", "start"]