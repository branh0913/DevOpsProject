FROM ubuntu:16.04
RUN apt-get update -qq
RUN apt-get -qq install wget net-tools iptables git vim  -y
RUN apt-get install software-properties-common -y
RUN add-apt-repository ppa:saltstack/salt -y
RUN apt-get install salt-minion -y
COPY ./files/minion /etc/salt/
