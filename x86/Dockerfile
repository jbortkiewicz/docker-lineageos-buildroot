FROM ubuntu:xenial

RUN apt-get update && apt-get install -y \
	bc \
	bison \
	build-essential \
	curl \
	flex \
	g++-multilib \
	gcc-multilib \
	git \
	gnupg \
	gperf \
	imagemagick \
	lib32ncurses5-dev \
	lib32readline-dev \
	lib32z1-dev \
	libesd0-dev \
	liblz4-tool \
	libncurses5-dev \
	libsdl1.2-dev \
	libssl-dev \
	libwxgtk3.0-dev \
	libxml2 \
	libxml2-utils \
	lzop \
	pngcrush \
	repo \
	rsync \
	schedtool \
	squashfs-tools \
	xsltproc \
	zip \
	zlib1g-dev
	
RUN     useradd -m -u 1000 lineage 

VOLUME /home/lineage
WORKDIR /home/lineage
USER lineage
ENTRYPOINT ["/bin/bash"]