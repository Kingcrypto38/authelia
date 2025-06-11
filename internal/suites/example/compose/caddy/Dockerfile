FROM caddy:2.7.6-builder AS builder

RUN xcaddy build fix-empty-copy-headers

FROM caddy:latest

COPY --from=builder /usr/bin/caddy /usr/bin/caddy
