FROM --platform=$BUILDPLATFORM maven:3.8.6-openjdk-11-slim as build

WORKDIR /app

COPY ./ ./

RUN mvn clean install

FROM --platform=$BUILDPLATFORM openjdk:11-jre-slim AS base

WORKDIR /app

COPY --from=build /app/target/demo-0.0.1-SNAPSHOT.jar app.jar

COPY entrypoint.sh ./

ENTRYPOINT ["sh", "/app/entrypoint.sh" ]
