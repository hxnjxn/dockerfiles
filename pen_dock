FROM ubuntu:latest
MAINTAINER jackson

WORKDIR /opt/

RUN apt-get update && apt-get install -y \
	build-essential \
	git-core \
	vim \
	wget \
	nfs-common \
	whois \
	snmp \
	ssh \
	curl \
	libssl-dev \
	
RUN git clone --depth=1 https://github.com/nmap/nmap.git && \
	cd nmap && \
	./configure --without-zenmap && \
	make && \
	make install && \
	rm -rf ../nmap
RUN git clone https://github.com/leebaird/discover \

