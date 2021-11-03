FROM node:14-slim

#Create wokring directory
WORKDIR /usr/src/app

#Copy package.json into working directory 
COPY ./package.json ./
COPY ./package-lock.json ./

#Install latest dependencies
RUN npm install

#copy rest of the source code into the current directory
COPY . .

EXPOSE 2000

CMD ["npm", "start"]
