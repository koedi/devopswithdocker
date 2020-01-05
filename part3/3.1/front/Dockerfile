FROM ubuntu:16.04

RUN apt update && \
    apt-get install -y git && \
    apt-get install -y curl && \
    apt-get install -y nodejs && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    git clone https://github.com/docker-hy/frontend-example-docker && \
    npm install && \
    apt-get purge -y --auto-remove curl && \
    rm -rf /var/lib/apt/lists/*

    
WORKDIR ./frontend-example-docker

EXPOSE 5000

CMD ["npm","start"]
