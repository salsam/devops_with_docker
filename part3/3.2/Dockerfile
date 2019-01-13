FROM alpine:3.7

WORKDIR /app

RUN apk add --update --no-cache gcc python3 python3-dev libc-dev libxslt-dev wget && \
    pip3 install --user --upgrade yle-dl

ENTRYPOINT read url;sleep 1;python3 ~/.local/bin/yle-dl $url