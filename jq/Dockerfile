# echo '{"hello": "world"}' | docker run --rm -i jq .

FROM alpine:latest

RUN apk add --no-cache jq

ENTRYPOINT ["jq", "-C"]
