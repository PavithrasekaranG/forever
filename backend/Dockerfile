# Build stage
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy source code
COPY . .

# Expose port
EXPOSE 4000

# Environment variables
ENV PORT=4000
ENV MONGODB_URI=mongodb://mongo:27017
ENV CLOUDINARY_NAME=your_cloudinary_name
ENV CLOUDINARY_API_KEY=your_cloudinary_api_key
ENV CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key
ENV JWT_SECRET=your_jwt_secret_key
ENV ADMIN_EMAIL=admin@example.com
ENV ADMIN_PASSWORD=admin_password

# Start the server
CMD ["npm", "start"]
