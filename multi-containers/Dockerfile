# Use an official Node runtime as a parent image
FROM node:alpine

# Set the working directory in the container
WORKDIR /usr/app

# Copy package.json and package-lock.json to the working directory
COPY package.json .

# Install any needed packages specified in package.json
RUN npm install

# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY ./ ./

# Debug step: list the contents of /usr/app
RUN ls -la /usr/app

# Make port 3000 available to the world outside this container
#EXPOSE 3000

# Define environment variable
#ENV NODE_ENV=production

# Run the app when the container launches
CMD ["npm", "start"]
