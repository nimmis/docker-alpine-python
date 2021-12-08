FROM nimmis/alpine-micro

MAINTAINER nimmis <kjell.havneskold@gmail.com>


RUN apk update && apk upgrade && \
    apk add python2 && \
    apk add --virtual=build-dependencies curl && \
    curl https://bootstrap.pypa.io/pip/2.7/get-pip.py | python && \
    apk del build-dependencies && \
    rm -Rf /root/.cache && \
    rm -rf /var/cache/apk/*


