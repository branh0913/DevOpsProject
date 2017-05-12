FROM ubuntu:16.04
RUN apt-get update -qq
RUN apt-get install -y -qq  net-tools apt-utils iptables wget vim
RUN wget -O - https://repo.saltstack.com/apt/ubuntu/16.04/amd64/latest/SALTSTACK-GPG-KEY.pub | apt-key add -
RUN echo 'deb http://repo.saltstack.com/apt/ubuntu/16.04/amd64/latest xenial main' > /etc/apt/sources.list.d/saltstack.list
RUN apt-get update -qq
RUN apt-get install salt-master -y -qq
RUN apt-get install python-pygit2 -y -qq
