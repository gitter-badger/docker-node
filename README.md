NodeJS run by nodemon, with bower and sass
---

[![Join the chat at https://gitter.im/konder/docker-node](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/konder/docker-node?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

# BUILD your image

```shell
FROM konder/node
MAINTAINER konder "konders@gmail.com"

ADD . /src
RUN cd /src; npm install

EXPOSE 3000

CMD [ "nodemon", "/src/app.js" ]
```
