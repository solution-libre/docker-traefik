# Traefik with Docker Compose

<!-- markdownlint-disable-next-line MD001 -->
#### Table of Contents

1. [Description](#description)
2. [Setup](#setup)
3. [Usage](#usage)
4. [Reference](#reference)
5. [Development](#development)
6. [Contributors](#contributors)

## Description

[Docker Compose](https://docs.docker.com/compose/) setup for starting [Traefik](https://traefik.io/)
with [Let's Encrypt](https://letsencrypt.org/) by [Solution Libre].

## Setup

1. Create an external network:

    ```sh
    docker network create web
    ```

2. Clone this repo:

    ```sh
    cd /opt
    git clone https://usine.solution-libre.fr/docker/traefik.git
    cd traefik
    ```

3. Declare environment variables or copy the `.env.dist` to `.env` and adjust its values.
4. Copy the `.env.traefik.dist` to `.env.traefik` and adjust its values.

## Usage

```sh
cd /opt/traefik
docker compose up -d
```

For a service to be accessible through Traefik, it must:

1. Be connected to the Traefik network (default `web`)
2. Have the appropriate Docker labels

Example Docker Compose configuration for a service:

```yaml
services:
  myapp:
    image: myapp:latest
    networks:
      - web
    labels:
      - "traefik.enable=true"
      - "traefik.http.routers.myapp.rule=Host(`myapp.example.com`)"
      - "traefik.http.routers.myapp.entrypoints=websecure"
      - "traefik.http.routers.myapp.tls.certresolver=myresolver"
      - "traefik.http.services.myapp.loadbalancer.server.port=80"

networks:
  proxy:
    external: true
```

## Reference

See [REFERENCE.md](./REFERENCE.md).

## Development

[Solution Libre]'s repositories are open projects,
and community contributions are essential for keeping them great.

[Fork this repo on our GitLab](https://usine.solution-libre.fr/docker/traefik/-/forks/new) or
[on GitHub](https://github.com/solution-libre/docker-traefik/fork)

## Contributors

The list of contributors can be found at: <https://usine.solution-libre.fr/docker/traefik/-/graphs/main>

[Solution Libre]: https://www.solution-libre.fr
