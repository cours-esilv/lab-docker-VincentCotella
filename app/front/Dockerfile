# Use Nginx as the base image
FROM nginx:latest

# Copy your HTML files and any other assets into the container
COPY . /usr/share/nginx/html

# Set the environment variable for the back-end URL
ENV WS_BACK_URL http://e9e04ad2b2ea:8080

# Expose the port on which Nginx will listen
EXPOSE 80

# Define an entrypoint to start the web server
ENTRYPOINT ["nginx", "-g", "daemon off;"]
