FROM node:18.13.0-alpine

ARG WORKDIR

ENV HOME=/${WORKDIR}

WORKDIR ${HOME}

RUN apk update
CMD ["npm", "run", "dev"]
