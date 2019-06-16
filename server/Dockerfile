FROM node:8-alpine

RUN adduser -D legodi && mkdir /app && apk add make gcc g++ && apk add python
WORKDIR  /app
COPY . .
RUN npm install && chown -R legodi /app
USER legodi
EXPOSE 3001
CMD [ "npm", "start" ]
