# docker run -v $(pwd):/code --rm -it jolexa/wormhole
FROM python:alpine
# libffi is a runtime dependency
RUN apk --update add --virtual \
    build-dependencies openssl-dev build-base \
    && apk add libffi-dev \
    && pip install magic-wormhole==0.9.2 && mkdir /code \
    && apk del build-dependencies
WORKDIR /code
ENTRYPOINT ["wormhole"]
