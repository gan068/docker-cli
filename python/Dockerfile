FROM --platform=$BUILDPLATFORM python:3.8.13-alpine3.16

WORKDIR /app

COPY src ./

RUN pip install -r requirements.txt

ENTRYPOINT [ "python" ]
