# Define what image you want to build from 
# Here we use version 10 of node, available from Docker Hub 
FROM node:10

# Create app directory to hold the application code inside the image
# This will be the working directory for your application 
WORKDIR /C:/Users/s120748/OneDrive/transformation/github_jenkins_docker/ 

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

# RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]