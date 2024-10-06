FROM alpine:3.20

RUN apk add --no-cache \
    openrc \
    znc

# RUN addgroup -S znc && adduser -S znc -G znc

WORKDIR /app

USER znc

EXPOSE 1025 6667

CMD ["znc", "--foreground"]
