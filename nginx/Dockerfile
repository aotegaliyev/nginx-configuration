FROM nginx:latest

COPY nginx.conf /etc/nginx/nginx.conf
COPY sites-enabled/ /etc/nginx/sites-enabled/

RUN apt-get update && \
    apt-get install -y certbot python3-certbot-nginx && \
    rm /etc/nginx/conf.d/default.conf
