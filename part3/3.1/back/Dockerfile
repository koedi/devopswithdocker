FROM ubuntu:16.04

WORKDIR ./backend-example-docker

RUN apt-get update && \
    apt-get install -y curl && \
    apt-get install -y git && \
    #apt-get install -y npm && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs && \
    git clone https://github.com/docker-hy/backend-example-docker && \
    npm install && \
    apt-get purge -y --auto-remove curl && \
    rm -rf /var/lib/apt/lists/*


EXPOSE 8000

CMD ["npm", "start"]
