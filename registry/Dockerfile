FROM registry:2.8.3

COPY config.yml /etc/docker/registry/config.yml

EXPOSE 5000

VOLUME ["/var/lib/registry"]

CMD ["/etc/docker/registry/config.yml"]
