# Nodejs sample

## build

`docker build -t user/node:latest -f ./Dockerfile .`

## run

`docker run  --rm user/node:latest /app/string-util.js help split`
`docker run  --rm user/node:latest /app/string-util.js split a,b,c`
