FROM node:alpine

RUN apk add --no-cache git && \
    git clone https://github.com/docker-hy/backend-example-docker && \
    adduser -D app && \
    chown -R app /backend-example-docker

USER app

WORKDIR ./backend-example-docker

RUN npm install

EXPOSE 8000
ENV FRONT_URL=http://localhost:5000


CMD ["npm", "start"]
