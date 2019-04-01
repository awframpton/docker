FROM local/c7-systemd

COPY neotechnology.gpg.key /tmp
COPY neo4j.repo /etc/yum.repos.d

RUN rpm --import /tmp/neotechnology.gpg.key; \
  yum -y install neo4j; \
  systemctl enable neo4j

CMD ["/usr/sbin/init"]
