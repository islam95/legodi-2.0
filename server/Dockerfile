FROM node:8-alpine

RUN adduser -D legodi && mkdir /app && chown -R legodi /app
USER legodi
WORKDIR  /app
COPY . .
RUN apk add make gcc g++ && apk add python
RUN npm install
EXPOSE 3001
CMD [ "npm", "start" ]
