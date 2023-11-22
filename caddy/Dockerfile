FROM caddy:2.7.5-builder AS builder
RUN xcaddy build --with github.com/porech/caddy-maxmind-geolocation \
                 --with github.com/caddyserver/transform-encoder \
                 --with github.com/caddy-dns/google-domains
                 
FROM caddy:2.7.5
COPY --from=builder /usr/bin/caddy /usr/bin/caddy