FROM ubuntu:16.04

RUN apt update && apt install -y git

RUN apt update && apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt update && apt install -y nodejs
RUN git clone https://github.com/docker-hy/frontend-example-docker


WORKDIR ./frontend-example-docker

RUN npm install

EXPOSE 5000

CMD ["npm","start"]
