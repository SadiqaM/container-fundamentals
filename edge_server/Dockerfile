
# Use a slim base image for Nginx
FROM nginx:stable-alpine3.19-slim
LABEL org.opencontainers.image.authors="Sadiqa M"
LABEL server_type="edge_server"
LABEL org.opencontainers.image.licenses=APACHE2
LABEL org.opencontainers.image.description="Containter Fundamentals - Static Website Image"

COPY config/nginx.conf /etc/nginx/
COPY web_content/ /var/www

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]