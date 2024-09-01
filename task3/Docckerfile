# use the latest nginx image
FROM nginx:latest

# Copie files in /var/www/html
COPY softy-pinko-front-end/ /var/www/html/softy-pinko-front-end/

# Copie files in /etc/nginx/conf.d/default.conf
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose le port 9000
EXPOSE 9000
