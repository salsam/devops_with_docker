from ubuntu:16.04

WORKDIR /curler
RUN apt update && apt install -y curl

CMD read website;sleep 3;curl http://$website;