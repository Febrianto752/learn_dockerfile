# FROM golang:1.18-alpine

# RUN mkdir app
# RUN addgroup -S developer
# RUN adduser -S -D -h /app febrianto developer 
# RUN chown -R febrianto:developer /app 
# USER febrianto

# COPY main.go /app/

# EXPOSE 8080

# CMD go run /app/main.go

FROM golang:1.18-alpine

RUN mkdir app 
RUN addgroup developer 
RUN adduser febrianto --disabled-password
RUN adduser febrianto developer
RUN ls
RUN chown -R febrianto:developer app

COPY main.go /app/

USER febrianto

EXPOSE 8080
CMD go run /app/main.go

