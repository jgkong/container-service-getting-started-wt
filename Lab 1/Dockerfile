FROM node:6
RUN apt-get update &&\
  apt-get clean &&\
  rm -Rf /var/cache/*
COPY package.json .
RUN npm install
COPY app.js .
EXPOSE  8080
CMD node app.js
