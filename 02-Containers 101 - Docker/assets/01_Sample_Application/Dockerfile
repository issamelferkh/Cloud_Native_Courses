FROM alpine:17-alpine3.14

RUN apk add python2 g++ make

COPY /app /app
RUN yarn install
CMD ["node", "src/index.js"]
EXPOSE 3000