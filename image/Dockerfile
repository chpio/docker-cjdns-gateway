FROM debian:jessie

RUN { \
	set -ex; \
	apt-get update; \
	apt-get install --no-install-recommends -y radvd; \
	rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*; \
}

COPY start-cjdns-gateway /usr/bin
CMD ["start-cjdns-gateway"]
