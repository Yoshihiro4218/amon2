FROM perl:5.24.1
LABEL maintainer "example"

WORKDIR /tmp

RUN apt-get update -y && \
	apt-get clean && \
	rm -fr /var/lib/apt/lists/*

RUN cpanm Carton

RUN useradd -d /home/docker -m -s /bin/bash -u 1000 -g 50 docker

RUN mkdir -p /data/www
VOLUME ["/data"]
WORKDIR /data/www

USER 1000

CMD ["perl","-v"]