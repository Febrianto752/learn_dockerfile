FROM golang:1.18-alpine 

ARG app=main 

RUN mkdir /app 
COPY main.go /app/
RUN mv /app/main.go /app/${app}.go 

EXPOSE 8080

ENV filename=${app}
CMD go run /app/${filename}.go