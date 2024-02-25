# Use a base Node.js image
FROM node:18.18.1

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json if applicable
COPY ./package*.json ./

# Install project dependencies
RUN npm install

# Copy the entire project
COPY . .

# Build the Vite.js project
# RUN npm run build

# Expose the port your app will run on
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]
