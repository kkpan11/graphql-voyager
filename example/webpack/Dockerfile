# syntax=docker/dockerfile:1

FROM node:20

WORKDIR /app

COPY ./graphql-voyager-*.tgz graphql-voyager.tgz

COPY ./example/webpack ./example/webpack

WORKDIR example/webpack
RUN npm install
RUN npm test

EXPOSE  9090
CMD npm start
