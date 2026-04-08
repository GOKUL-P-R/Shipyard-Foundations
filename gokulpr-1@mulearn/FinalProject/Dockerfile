# Use nginx:alpine as base image
FROM nginx:alpine

# Set working directory
WORKDIR /usr/share/nginx/html

# Copy index.html to nginx serving directory
COPY index.html .

# Expose port 80
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
