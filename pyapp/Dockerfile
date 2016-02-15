FROM undeadops/alpine-python

MAINTAINER Mitch Anderson <@undeadops>

RUN apk add --update \
  nginx \
  && mkdir -p /etc/nginx/sites-enabled \
  && mkdir -p /etc/nginx/ssl \
  && mkdir /source \
  && mkdir /www \
  && mkdir -p /var/log/nginx \
  && rm -rf /var/cache/apk/*

RUN ln -sf /dev/stdout /var/log/nginx/access.log
RUN ln -sf /dev/stderr /var/log/nginx/error.log

EXPOSE 80 443

CMD ["/usr/sbin/nginx". "-g", "daemon off;"]
