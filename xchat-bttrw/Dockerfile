FROM alpine:3.20 as builder

RUN apk add --no-cache \
    build-base \
    curl-dev \
    git

# Set working directory
WORKDIR /app

COPY ./src /app

RUN dos2unix /app/mkreadme

RUN make

EXPOSE 6669

CMD ["./gate"]
