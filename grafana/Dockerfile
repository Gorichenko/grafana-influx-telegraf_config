FROM grafana/grafana:4.4.2

RUN apt-get update && apt-get install -y curl gettext-base && rm -rf /var/lib/apt/lists/*

WORKDIR /etc/grafana
COPY datasources ./datasources

WORKDIR /var/www
COPY entrypoint.sh ./
RUN chmod u+x entrypoint.sh

ENTRYPOINT ["/var/www/entrypoint.sh"]
