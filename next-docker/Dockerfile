# Inherit from an official Node.js image
FROM node:20-alpine3.18

# Set the working directory in the container
WORKDIR /app

# Copy only package.json and package-lock.json to avoid conflicts
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files into the container, excluding those in .dockerignore
COPY . .

# Expose the port that the app runs on
EXPOSE 3000

# Start the application
CMD ["npm", "run", "dev"]




