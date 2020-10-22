FROM node:alpine

# set working directory for container
WORKDIR /usr/app

# Copy package.json first to avoid reinstalling packages when there are no changes
COPY ./package.json ./

# Install some dependencies
RUN npm install

# Copy remaining src items
COPY ./ ./

# Run command on container start
CMD ["npm", "start"]