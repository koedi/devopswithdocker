FROM ubuntu:16.04

COPY . .

RUN apt-get update && \
    apt-get install -y curl && \
    apt-get install -y git && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs && \
    git clone https://github.com/docker-hy/backend-example-docker && \
    apt-get purge -y --auto-remove curl && \
    rm -rf /var/lib/apt/lists/* && \
    useradd -m app && \
    chown app /backend-example-docker

USER app

WORKDIR ./backend-example-docker

RUN npm install

EXPOSE 8000

CMD ["npm", "start"]
