# Use Node base image
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy all other files
COPY . .

# Expose the port your app runs on
EXPOSE 5173

# Run the dev server (Vite)
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]

