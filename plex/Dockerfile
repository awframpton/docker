FROM ubuntu:18.04

COPY plex.deb /tmp

RUN dpkg -i /tmp/plex.deb && rm -f /tmp/plex.deb

EXPOSE 32400

CMD ["su", "plex", "-c", "/usr/sbin/start_pms"]
