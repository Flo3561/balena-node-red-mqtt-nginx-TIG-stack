FROM nodered/node-red:latest

## installing an editor
#USER root
#RUN apt-get update && apt-get install nano
USER node-red

RUN npm install node-red-contrib-resinio \
    node-red-contrib-credentials \
    node-red-contrib-moment \
    node-red-contrib-config \
    node-red-contrib-fs-ops \
    node-red-contrib-http-multipart \
    node-red-contrib-md5 \
    node-red-contrib-ui_list \
    node-red-dashboard

## install node-red-admin which is needed if you want to created hashed password for the node-red editor.
#RUN sudo npm install -g --unsafe-perm node-red-admin

COPY ./settings.js /data/settings.js
