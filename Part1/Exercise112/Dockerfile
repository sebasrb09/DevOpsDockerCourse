FROM ubuntu:16.04


RUN apt-get update
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt install -y nodejs

RUN echo "Node: " && node -v
RUN echo "NPM: " && npm -v

WORKDIR /usr/src/app

COPY package*.json ./

COPY . .

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD ["serve","-s","-l", "5000" ,"build"]