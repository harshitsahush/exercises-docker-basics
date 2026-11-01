FROM ubuntu:24.04
WORKDIR /usr/src/app
RUN apt-get update
RUN apt-get install curl -y
COPY script.sh .
CMD ["./script.sh"]
