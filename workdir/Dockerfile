FROM golang:1.18-alpine

ENV APP_PORT=8080

RUN mkdir app
WORKDIR /app
COPY main.go ./

EXPOSE ${APP_PORT}

CMD go run main.go