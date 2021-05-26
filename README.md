# Træfik with Docker Compose

#### Table of Contents

1. [Description](#description)
2. [Setup](#setup)
3. [Usage](#usage)
4. [Reference](#reference)
5. [Development](#development)
6. [Contributors](#contributors)

## Description

[Docker Compose](https://docs.docker.com/compose/) setup for starting [Træfik](https://traefik.io/) with [Let's Encrypt](https://letsencrypt.org/).

## Setup

Create an external network:

```sh
docker network create web
```

Clone this repo:

```sh
cd /opt
git clone https://github.com/solution-libre/docker-traefik.git traefik
cd traefik
```

Declare environment variables or copy the `.env.dist` to `.env` and adjust its values.

## Usage

```sh
cd /opt/traefik
docker-compose up -d
```

## Reference

### Environment variables

#### `ACME_EMAIL`

Email address used for ACME registration. Default value: 'webmaster@my.domain.tld'

#### `DEFAULT_DOMAIN`

Default TLS domains.
Default value: 'my.domain.tld'

#### `HTTP_PORT`

HTTP listen port.
Default value: 80

#### `HTTPS_PORT`

HTTPs listen port.
Default value: 443

## Development

[Solution Libre](https://www.solution-libre.fr)'s repositories are open projects, and community contributions are essential for keeping them great.

[Fork this repo on GitHub](https://github.com/solution-libre/docker-traefik/fork)

## Contributors

The list of contributors can be found at: <https://github.com/solution-libre/docker-traefik/graphs/contributors>
