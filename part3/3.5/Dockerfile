FROM node:alpine as build-stage

RUN apk add --no-cache git && \
    git clone https://github.com/docker-hy/frontend-example-docker

WORKDIR ./frontend-example-docker

RUN npm install
RUN npm run build

FROM nginx
COPY --from=build-stage /frontend-example-docker/dist /usr/share/nginx/html
