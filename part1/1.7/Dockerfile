FROM ubuntu:22.04

WORKDIR /usr/src/app

RUN apt update 
RUN apt install curl -y
COPY script.sh .

RUN chmod +x script.sh

ENTRYPOINT ["./script.sh"]
