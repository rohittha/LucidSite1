# Use the official Nginx image from Docker Hub
FROM nginx:alpine

# Explicitly remove the default Nginx files first
RUN rm -rf /usr/share/nginx/html/*

# Copy your website files into the Nginx html directory
COPY . /usr/share/nginx/html

# Expose port 80 (the default Nginx port)
EXPOSE 80

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]