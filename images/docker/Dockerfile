
FROM antidotelabs/utility

RUN apt-get install lsb-release -y
RUN apt-get install software-properties-common -y
RUN apt-get install apt-transport-https -y

RUN curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add - && \
    add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" && \
    apt-get update

RUN apt-cache policy docker-ce
RUN apt-get install -y docker-ce

#RUN groupadd docker
RUN usermod -aG docker antidote
RUN systemctl enable docker

RUN mkdir /home/antidote/.docker
#RUN chown antidote:antidote /home/antidote/.docker -R
RUN chown -R antidote:antidote /home/antidote/.docker
#RUN chmod g+rwx /home/antidote/.docker -R
RUN chmod -R 777 /home/antidote/.docker


#RUN gpasswd -a antidote docker
#RUN newgrp docker

COPY ./docker_configs/Dockerfile /home/antidote
