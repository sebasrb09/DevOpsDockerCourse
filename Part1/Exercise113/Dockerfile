FROM golang:1.16-alpine

RUN apk add build-base

WORKDIR /app

COPY go.mod ./
COPY go.sum ./

EXPOSE 8000

COPY . . 

RUN echo go version

RUN go build

RUN go test


CMD [ "./server","--port=8000"]