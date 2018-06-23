FROM daocloud.io/node:4.8
LABEL maintainer = 'shutiao'
EXPOSE 8888
RUN mkdir -p /usr/voting-app/
WORKDIR /usr/voting-app/
COPY package.json /usr/voting-app/
RUN npm install
CMD ["npm", "start"]
VOLUME /usr/voting-app/src/
