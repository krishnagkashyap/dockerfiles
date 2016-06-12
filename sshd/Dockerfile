FROM	ubuntu
MAINTAINER	Krishna Kashyap <krishnagkashyap@gmail.com>

RUN apt-get update -y && apt-get upgrade -y && apt-get install -y openssh-server

RUN mkdir -p /var/run/sshd


RUN groupadd dba
RUN groupadd svrtech
RUN groupadd wheel

RUN useradd -md /u01 -G wheel,dba,svrtech -s /bin/bash usr0

# Print "Hello docker!"
RUN echo "Hello docker!"
