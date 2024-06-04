# Use the official NGINX image as the parent image
FROM nginx:alpine

# Copy the nginx.conf and default.conf to the appropriate location
COPY nginx.conf /etc/nginx/nginx.conf
COPY default.conf /tmp/default.conf

# Copy the start.sh script to the container
COPY start.sh /start.sh

# Make start.sh executable
RUN chmod +x /start.sh

# Expose port 80
EXPOSE 80

# Run the start.sh script
CMD ["sh","/start.sh"]
