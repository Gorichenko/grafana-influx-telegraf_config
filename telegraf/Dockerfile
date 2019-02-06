FROM telegraf:latest

COPY telegraf.conf ./etc/telegraf/telegraf.conf
COPY entrypoint.sh ./
RUN chmod u+x entrypoint.sh

EXPOSE 8125/udp 8092/udp 8094

ENTRYPOINT ["/entrypoint.sh"]