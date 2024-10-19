FROM node:18-alpine

ENV YARN_VERSION=4.5.1
RUN apk update \
 && apk add lftp \
 && apk search git \
 && apk add git \
 && yarn set version ${YARN_VERSION}

ENTRYPOINT ["docker-entrypoint.sh"]
CMD [ "node" ]