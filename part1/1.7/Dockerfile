FROM ubuntu:16.04

WORKDIR /home/kpietika/Documents/Opinnot/Docker/part1/1.7


RUN apt-get update && apt-get install -y curl
COPY curler.sh .
RUN chmod +x curler.sh
CMD ["/bin/sh", "-c", "./curler.sh"]
