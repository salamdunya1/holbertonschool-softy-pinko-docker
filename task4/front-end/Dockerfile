# Use the latest Nginx image as the base
FROM nginx:latest

# Copy the front-end files to the appropriate directory in the Nginx image
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file to the appropriate directory
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
