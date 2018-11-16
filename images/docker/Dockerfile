FROM antidotelabs/utility

RUN curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && \
    add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" && \
    apt-get update

RUN apt-cache policy docker-ce
RUN sudo apt-get install -y docker-ce

COPY ./docker_configs/Dockerfile .