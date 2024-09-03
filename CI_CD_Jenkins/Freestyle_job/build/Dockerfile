FROM alpine:latest

WORKDIR /web_app

RUN apk update && \
    apk add nginx

ENTRYPOINT ["tail", "-f", "/dev/null"]    

COPY ../nginx/index.html /var/www/html/index.html

COPY ../nginx/default.conf /etc/nginx/http.d/default.conf

CMD ["nginx", "-g", "daemon off;"]
