# FROM debian:stretch-slim as builder
FROM python:3
MAINTAINER Felipe Villalobos <fvillalobos@medioclick.com>

# RUN groupadd -r -g 1005 demohunter && \
#     useradd -r -u 1005 -d /demohunter -m -g demohunter demohunter

# Set up Debian prereqs
RUN export DEBIAN_FRONTEND=noninteractive; \
    apt-get update && \
    apt-get install -y \
        -o APT::Install-Suggests=false \
        -o APT::Install-Recommends=false \
        #python3.5 \
        #python3.5-dev \
        python-dev \
        git
      #python-pip \
      #libssl-dev \
      #libffi-dev \
      #build-essential \
      # virtualenv \
      # python-virtualenv


# RUN su - demohunter -c
RUN python3 --version
RUN pip install setuptools
RUN pip install git+https://github.com/RevengeComing/DemonHunter.git

#USER demohnunter
WORKDIR /opt/demohunter

EXPOSE 8000
#ENTRYPOINT ["/bin/bash", "-c", "dh_run"]
CMD ["/bin/bash", "-c", "dh_run"]
