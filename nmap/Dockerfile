# Add to PATH, like this:
# echo 'docker run -it --rm jolexa/nmap $@' > ~/bin/nmap

FROM alpine:3.7

RUN apk add --update --no-cache nmap
ENTRYPOINT ["/usr/bin/nmap"]
CMD ["--help"]
