FROM --platform=$BUILDPLATFORM node:18.12.0-alpine3.16

WORKDIR /app

COPY src ./

RUN npm ci

ENTRYPOINT [ "node" ]
