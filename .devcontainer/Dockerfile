FROM debian:12-slim

# Use apt-get to install wget 
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install git -y
RUN apt-get install openssh-server -y 
RUN apt-get install sudo locales -y
RUN apt-get install sudo -y
RUN apt-get clean

RUN useradd -rm -d /home/student -s /bin/bash -g root -G sudo -u 1001 --disabled-password --gecos '' student
USER student
WORKDIR /home/student
