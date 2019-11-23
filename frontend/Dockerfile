FROM ubuntu:16.04
COPY . /home/
WORKDIR /home/
RUN apt update -y
RUN apt install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
EXPOSE 5000
CMD API_URL=${API_URL} npm start