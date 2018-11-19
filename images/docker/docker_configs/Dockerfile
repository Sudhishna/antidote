FROM antidotelabs/utility

RUN wget -O - https://repo.saltstack.com/apt/ubuntu/16.04/amd64/archive/2018.3.2/SALTSTACK-GPG-KEY.pub | apt-key add - && \
    echo "deb http://repo.saltstack.com/apt/ubuntu/16.04/amd64/archive/2018.3.2 xenial main" >> /etc/apt/sources.list && \
    apt-get update
RUN apt-get --auto-remove --yes remove python-openssl
RUN pip install pyOpenSSL
RUN pip install jxmlease

RUN apt-get install -y salt-master
RUN apt-get install -y salt-minion