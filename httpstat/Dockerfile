FROM golang:alpine
LABEL maintainer="Ricardo Rebello Sierra <contato@ricardosierra.com.br>"


## https://github.com/davecheney/httpstat
# httpstat() {
#   docker run -it --rm \
#     ondrejmo/httpstat "$@"
# }

RUN apk update && apk add git \
  && rm -rf /var/cache/apk/*
RUN go get -u github.com/davecheney/httpstat

ENTRYPOINT [ "httpstat" ]
