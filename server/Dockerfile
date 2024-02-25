# Use a base Node.js image
FROM node:18.18.1

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port your app will run on
EXPOSE 4000

# Command to run the application
CMD ["npm", "start"]
