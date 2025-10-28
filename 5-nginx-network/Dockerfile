FROM nginx:1.29.2-alpine

COPY index.html /usr/share/nginx/html
COPY default.conf /etc/nginx/conf.d/default.conf
EXPOSE 80

# docker run --name nginx-demo -p 8081:80 -d nginx