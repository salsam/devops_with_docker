from ubuntu:16.04

WORKDIR /backend-example-docker
COPY . .

RUN apt update && apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install

EXPOSE 8000

ENTRYPOINT npm start