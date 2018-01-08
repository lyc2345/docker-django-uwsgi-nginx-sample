FROM nginx:latest

COPY nginx.conf /etc/nginx/nginx.conf
COPY my_nginx.conf /etc/nginx/sites-avaliable/

RUN mkdir -p /etc/nginx/sites-enabled/ \
  && ln -s /etc/nginx/sites-avaliable/my_nginx.conf /etc/nginx/sites-enabled/

CMD ["nginx", "-g", "daemon off;"]
