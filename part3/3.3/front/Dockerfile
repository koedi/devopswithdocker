FROM ubuntu:16.04


RUN apt update && \
    apt-get install -y git && \
    apt-get install -y curl && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs && \
    git clone https://github.com/docker-hy/frontend-example-docker && \
    apt-get purge -y --auto-remove curl && \
    rm -rf /var/lib/apt/lists/* && \
    useradd -m app && \
    chown app -R /frontend-example-docker


WORKDIR ./frontend-example-docker
RUN npm install

EXPOSE 5000
ENV API_URL=http://localhost:8000
USER app

CMD ["npm","start"]
