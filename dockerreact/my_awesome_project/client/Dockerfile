#https://nodejs.org/en/docs/guides/nodejs-docker-webapp/
FROM node:14

#set working directory
WORKDIR /client

#copy package json into container
COPY package*.json /client/

# install dependencies
RUN npm install

# Copy the current directory contents into the container at /client
COPY . /client/

# Make port 3000 available to the world outside this container
EXPOSE 3000

# Run the app when the container launches
CMD ["npm", "start"]
