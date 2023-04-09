``` sh
docker-compose run front npm cache clean --force
docker-compose run front npm create vite@latest
cp -r ./front/app/project/. ./front/app/
docker-compose run front npm install
```

``` Dockerfile
FROM node:18.13.0-alpine

ARG WORKDIR

ENV HOME=/${WORKDIR}

WORKDIR ${HOME}

RUN apk update
# ADD
CMD ["npm", "run", "dev"]
```

``` sh
docker-compose stop
docker-compose build --no-cache
docker-compose up -d
```
