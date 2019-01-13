FROM ubuntu:18.04

WORKDIR /work

RUN apt update && \
    apt install -y \
    wget curl git python3 python3-pip clang-format-6.0

RUN pip3 install --upgrade pip && \
    pip install \ 
    ipython pylint


ENTRYPOINT "/bin/bash"