ARG ALPINE_VERSION=3.19

FROM alpine:${ALPINE_VERSION}

LABEL dev="Ramon"

ENV HOST="0.0.0.0"
#1
RUN apk add --no-cache nodejs

#2
RUN apk add --no-cache npm

#3
RUN apk add --no-cache git

#4
RUN apk add --no-cache wget

#5
RUN apk add --no-cache express

WORKDIR /opt/etc

ENTRYPOINT [ "node" ]

CMD [ "node" ]
