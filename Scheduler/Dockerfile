FROM alpine:3.9
ENV LIBRARY_PATH=/lib:/usr/lib
RUN apk add --no-cache --virtual .build-deps linux-headers alpine-sdk libjpeg-turbo-dev zlib-dev g++ python3-dev openssl-dev && \
    apk add --no-cache --update python3 && \
    pip3 install --upgrade pip setuptools && \
    pip3 install --upgrade dask distributed bokeh

EXPOSE 8787
ENTRYPOINT [ "dask-scheduler" ]