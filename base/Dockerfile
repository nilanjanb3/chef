FROM ubuntu:18.04

RUN useradd -rm -d /home/nilanjan -s /bin/bash -g root -G sudo -u 1001 nilanjan
RUN echo 'nilanjan:nilanjan' | chpasswd
WORKDIR /home/nilanjan
RUN apt update -y
RUN apt upgrade -y
RUN apt install ssh -y
RUN apt install openssh-server -y
RUN echo "PasswordAuthentication yes" >> /etc/ssh/sshd_config
RUN echo "PermitRootLogin yes" >> /etc/ssh/sshd_config
RUN echo 'root:root' | chpasswd
RUN service ssh start
RUN apt install sudo

CMD ["/usr/sbin/sshd","-D"]