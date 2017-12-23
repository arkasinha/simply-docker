FROM node:latest

#set working directory
RUN mkdir /usr/src/app
WORKDIR /usr/src

# add `/usr/src/node_modules/.bin` to $PATH
ENV PATH /usr/src/node_modules/.bin:$PATH

# add package.json
ADD package.json /usr/src/package.json
RUN npm install

# start app
CMD ["npm", "start"]