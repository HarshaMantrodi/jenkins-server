# Use official Node.js LTS image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files first to leverage Docker cache
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the project files
COPY . .

# Expose the app port
EXPOSE 3000

# Run the application
CMD ["npm", "start"]
