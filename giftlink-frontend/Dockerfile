# Step 1: Use the official Node.js image as a parent image
FROM node:16 AS build

# Step 2: Set the working directory
WORKDIR /app

# Step 3: Copy package.json and package-lock.json
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy the rest of your application code
COPY . .

# Step 6: Build the React app
RUN npm run build

# Step 7: Use a lightweight web server to serve the app
FROM nginx:alpine

# Step 8: Copy the build output to the Nginx html directory
COPY --from=build /app/build /usr/share/nginx/html

# Step 9: Expose the port Nginx is running on
EXPOSE 9000

# Step 10: Start Nginx server
CMD ["nginx", "-g", "daemon off;"]