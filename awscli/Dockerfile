# alias aws="docker run -it --rm -v $HOME/.aws/:/root/.aws jolexa/awscli --profile profile_name"
FROM python:alpine
RUN apk --no-cache add make zip && \
	pip install awscli==1.11.107
ENTRYPOINT ["aws"]
