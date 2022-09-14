FROM ubuntu
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && \
    apt-get -y install gcc mono-mcs && \
    rm -rf /var/lib/apt/lists/*
WORKDIR /src
COPY . /src
ENTRYPOINT ["gcc"]
CMD ["a.c"]
