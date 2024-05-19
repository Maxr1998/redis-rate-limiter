FROM redis:6-alpine

ARG TARGETARCH

COPY ratelimit-$TARGETARCH.so /usr/local/lib/ratelimit.so
COPY redis.conf /usr/local/etc/redis/redis.conf

CMD [ "redis-server", "/usr/local/etc/redis/redis.conf" ]