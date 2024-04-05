# Use official Node.js image as the base image
FROM node

# Set working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy application code to container
COPY . .

# Expose port 3000 to the outside world
EXPOSE 3000

# Command to run the Node.js application
CMD ["npm", "start"]