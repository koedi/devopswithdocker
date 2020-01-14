FROM ubuntu:16.04

WORKDIR /mydir

RUN apt update && \
    apt install -y gcc && \
    apt install -y emacs && \
    apt install -y git && \
    useradd -m dev && \
    chown dev -R /mydir

USER dev

CMD ["/bin/bash"]
