FROM node:alpine

RUN npm install --global @sanity/cli

RUN mkdir /app
ADD . /app

WORKDIR /app
RUN yarn

EXPOSE 3333

CMD ["/usr/local/bin/sanity", "start", "--host=0.0.0.0"]
