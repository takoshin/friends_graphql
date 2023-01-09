FROM golang:1.19-alpine

WORKDIR /go/src/app

ENV GO111MODULE=on

RUN apk add --no-cache \
        alpine-sdk \
        git \
    && go install github.com/pilu/fresh@latest

EXPOSE 8080

CMD ["fresh"]