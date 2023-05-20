FROM node:16-alpine

RUN set -eux \
    & apk add \
        --no-cache \
        yarn

WORKDIR /app

COPY package.json ./

RUN yarn

COPY . .

EXPOSE 5173

CMD [ "npm", "run", "dev" ]