FROM centos
RUN mkdir -p /var/run/sshd && yum -y update && yum -y install openssh-server
RUN ssh-keygen -A
ADD authorized_keys /root/.ssh/authorized_keys
CMD ["/usr/sbin/sshd", "-D"]
