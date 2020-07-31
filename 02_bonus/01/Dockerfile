FROM alpine

RUN apk update && apk upgrade && apk add yarn

ENTRYPOINT yarn --version

# docker build -t yarn .
# docker run -it --rm yarn