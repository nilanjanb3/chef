FROM ubuntu:18.04

RUN useradd -rm -d /home/nilanjan -s /bin/bash -g root -G sudo -u 1001 nilanjan -p nilanjan
WORKDIR /home/nilanjan
RUN  apt update -y
RUN  apt upgrade -y
RUN  apt install ssh -y
RUN  service ssh start

CMD ["sleep", "infinity"]