FROM bitnami/minideb:jessie  
USER root
ENV LANG C.UTF-8
RUN apt-get update
RUN apt-get install -y wget

RUN mkdir /sdomotica
COPY sdomotica /sdomotica

RUN chmod a+x /sdomotica/sdomotica

#-- Sdomotica interface is available on 3010
EXPOSE 3100 3000 3300

CMD ./sdomotica/sdomotica


