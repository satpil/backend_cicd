FROM node:latest
# node image:latest

WORKDIR /usr/src/app
# create a new working directory in container

COPY ./package*.json /usr/src/app
# copy the current dir package with wildcard  to the new working directory

RUN npm install
#install the dependencies

COPY . .
#copy all file in current dir to the new working directory

EXPOSE 3000
# expose the port to 3000

CMD [ "node","index.js" ]
#run the server
