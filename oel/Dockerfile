FROM oraclelinux:6.7

MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>

ADD oraclelinux-6.8-rootfs.tar.xz /

# overwrite this with 'CMD []' in a dependent Dockerfile
CMD ["/bin/bash"]


RUN yum update -y && yum  upgrade -y && yum  install -y openssh-server

#RUN mkdir -p /var/run/sshd


#RUN groupadd dba
#RUN groupadd svrtech
#RUN groupadd wheel

#RUN useradd -md /u01 -G wheel,dba,svrtech -s /bin/bash usr0

# Print "Hello docker!"
RUN echo "Hello docker!"
