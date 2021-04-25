FROM centos:latest
RUN yum install openssh-server passwd -y
RUN  echo root | passwd --stdin root
RUN ssh-keygen -A
CMD ["/usr/sbin/sshd", "-D"] && /bin/bash
