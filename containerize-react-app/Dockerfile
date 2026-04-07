# Use the base image form Docker Hub
FROM node:20-alpine

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose the port that the React app will run on
EXPOSE 5173

# Start the React app
CMD ["npm", "run", "dev"]