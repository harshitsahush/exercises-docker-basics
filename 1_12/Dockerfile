FROM ubuntu:latest
WORKDIR /usr/src/app

RUN apt update && apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt install -y nodejs

COPY . .

RUN npm install
RUN npm run build
RUN npm install -g serve

CMD ["serve", "-s", "-l", "5001", "build"]
