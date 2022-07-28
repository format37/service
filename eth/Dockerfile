FROM ubuntu:latest
WORKDIR /worker
# https://www.bminer.me/releases/
RUN  apt-get update \
  && apt-get install -y wget \
  && apt-get install xz-utils \
  && rm -rf /var/lib/apt/lists/* \
  && wget https://www.bminercontent.com/releases/bminer-v16.4.11-2849b5c-amd64.tar.xz \
  && tar -xpJf bminer-v16.4.11-2849b5c-amd64.tar.xz
ENTRYPOINT [ "/bin/bash", "-l", "-c" ]
CMD ["bminer-v16.4.9-c80288d/bminer $PARAM"]
#CMD ["sleep infinity"]