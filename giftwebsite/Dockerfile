FROM node:14 AS frontend-build
WORKDIR /usr/src/frontend
COPY ./giftlink-frontend ./
RUN npm install && npm run build


# Use Node.js LTS version
FROM node:14.17.0-slim

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json files
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy application code
COPY . .

# Copy the frontend build from the previous stage
COPY --from=frontend-build /usr/src/frontend/build ./build

# Expose port (if needed)
EXPOSE 9000

# Run the application
CMD ["node", "index.js"]