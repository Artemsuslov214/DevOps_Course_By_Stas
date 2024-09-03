FROM alpine:latest

WORKDIR /web_app

RUN apk update && \
    apk add nginx

#CMD ["tail", "-f", "/dev/null"] 
#CMD ["/bin/bash", "sleep", "200"]
#ENTRYPOINT ["tail", "-f", "/dev/null"]    
CMD ["/bin/bash", "-c", "ls -Rla"]

#COPY ../nginx/index.html /var/www/html/index.html

#COPY ../nginx/default.conf /etc/nginx/http.d/default.conf

CMD ["nginx", "-g", "daemon off;"]
