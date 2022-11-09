# java spring boot docker cli sample
- [java spring boot docker cli sample](#java-spring-boot-docker-cli-sample)
  - [build](#build)
  - [run](#run)

## build

`docker build -t user/java:latest -f ./Dockerfile .`

## run

`docker run --rm user/java:latest java -jar /app/app.jar`
