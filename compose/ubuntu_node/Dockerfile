FROM ubuntu:16.04
#FROM ubuntu

RUN apt-get update && apt-get install -y \
    openssh-server \
    software-properties-common \
 && rm -rf /var/lib/apt/lists/*

RUN mkdir /var/run/sshd

EXPOSE 22

CMD ["/usr/sbin/sshd", "-D", "-e", "-vvv"]