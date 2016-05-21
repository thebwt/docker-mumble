FROM ubuntu:16.04
MAINTAINER Brandon Tomlinson ( thebwt@gmail.com )

RUN apt-get update && apt-get install -y \
    mumble-server \
 && rm -rf /var/lib/apt/lists/*

CMD murmurd -ini /mumble/mumble-server.ini -fg
