FROM node:alpine

RUN apk add --no-cache git && \
    git clone https://github.com/docker-hy/frontend-example-docker && \
    adduser -D app && \
    chown app -R /frontend-example-docker


WORKDIR ./frontend-example-docker

RUN npm install

EXPOSE 5000
ENV API_URL=http://localhost:8000
USER app

CMD ["npm","start"]
