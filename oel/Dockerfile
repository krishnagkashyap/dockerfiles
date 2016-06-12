FROM oraclelinux:6.7

MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>

# overwrite this with 'CMD []' in a dependent Dockerfile
CMD ["/bin/bash"]


RUN yum  install -y openssh-server htop netcat python perl netcat htop wget curl

RUN yum clean all
#RUN mkdir -p /var/run/sshd


RUN groupadd dba
RUN groupadd svrtech
#RUN groupadd wheel

RUN useradd -md /u01 -G wheel,dba,svrtech -s /bin/bash usr0

# Print "Hello docker!"
RUN echo "Hello docker!"

RUN yum clean all
