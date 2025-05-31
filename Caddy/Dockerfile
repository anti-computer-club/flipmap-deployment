# builds Caddy, which provides easy TLS
FROM caddy:2.9.1-builder AS builder

RUN xcaddy build 
#--with github.com/mholt/caddy-ratelimit maybe another time

FROM caddy:2.9.1

COPY Caddyfile /etc/caddy/Caddyfile

COPY --from=builder /usr/bin/caddy /usr/bin/caddy
