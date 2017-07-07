FROM alpine:latest

WORKDIR /code
RUN apk --no-cache add openssl && \
    wget https://github.com/gohugoio/hugo/releases/download/v0.24.1/hugo_0.24.1_Linux-64bit.tar.gz -O - | tar -xzf -
ENTRYPOINT ["./hugo"]

