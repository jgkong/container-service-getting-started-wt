FROM registry.ng.bluemix.net/ibmnode
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get -y upgrade &&\
  apt-get clean &&\
  rm -Rf /var/cache/*
COPY package.json .
RUN npm install
COPY app.js .
EXPOSE  8080
CMD node app.js
