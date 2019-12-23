FROM ubuntu:16.04

WORKDIR ./backend-example-docker
COPY . .

RUN apt update && apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt update && apt install -y nodejs

RUN apt update && apt install -y git 
RUN git clone https://github.com/docker-hy/backend-example-docker


RUN npm install

EXPOSE 8000

CMD ["npm", "start"]
