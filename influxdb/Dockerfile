FROM influxdb:1.3.1-alpine

WORKDIR /var/www
COPY entrypoint.sh ./
RUN chmod u+x entrypoint.sh

ENTRYPOINT ["/var/www/entrypoint.sh"]
