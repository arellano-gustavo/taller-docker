FROM ubuntu

RUN apt-get update
RUN apt-get -y install sudo
RUN apt-get -y install curl

RUN useradd -m ejemplo && echo "ejemplo:ejemplo" | chpasswd && adduser ejemplo sudo
RUN gpasswd -a ejemplo sudo

RUN su -l ejemplo

#RUN curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
#RUN sudo apt-get install -y nodejs

USER ejemplo
CMD /bin/bash
