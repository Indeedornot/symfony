FROM debian

RUN apt-get update
RUN apt-get -y install wget

RUN wget -O /var/dbgpProxy https://xdebug.org/files/binaries/dbgpProxy
RUN chmod 0777 /var/dbgpProxy
RUN chmod +x /var/dbgpProxy

CMD /var/dbgpProxy -i 0.0.0.0:9100 -s 127.0.0.1:443
