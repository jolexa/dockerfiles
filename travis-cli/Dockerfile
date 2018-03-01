FROM alpine:3.6

# Add to PATH, like this:
# echo 'docker run -it --rm -v $(pwd):/code -w /code -v $HOME/.travis:/root/.travis jolexa/travis-cli $@' > ~/bin/travis

# Skip installing gem documentation
RUN echo 'gem: --no-rdoc --no-ri' >> "$HOME/.gemrc"

RUN apk add --update --no-cache git build-base ruby-dev libffi-dev ruby-bundler ca-certificates && \
    gem install travis -v 1.8.8 && \
    rm /var/cache/apk/* && \
    rm -rf /usr/share/ri

ENTRYPOINT ["travis"]
