# Reference

| Name                 | Description                                             | Default value             | Enabled |
| -------------------- | ------------------------------------------------------- | ------------------------- | ------- |
| ACME_DNS_CHALLENGE   | Activate DNS-01 Challenge                               | `false`                   | true    |
| ACME_DNS_CHALLENGE_PROVIDER | Use a DNS-01 based challenge provider rather than HTTPs | `gandiv5`          | true    |
| ACME_EMAIL           | Email address used for ACME registration                | `webmaster@my.domain.tld` | true    |
| ACME_HTTP_CHALLENGE  | Activate HTTP-01 Challenge                              | `false`                   | true    |
| ACME_TLS_CHALLENGE   | Activate TLS-ALPN-01 Challenge                          | `true`                    | true    |
| DEFAULT_DOMAIN       | Default TLS domains                                     | `my.domain.tld`           | true    |
| HTTP_PORT            | HTTP listen port                                        | `80`                      | true    |
| HTTPS_PORT           | HTTPs listen port                                       | `443`                     | true    |
| NETWORK_NAME         | External network name                                   | `web`                     | true    |
| VERSION              | Tag of the Docker image of Traefik                      | `v3.1`                    | true    |
