# Træfik with Docker

#### Table of Contents

1. [Description](#module-description)
2. [Setup](#setup)
3. [Usage](#usage)
4. [Development](#development)
5. [Contributors](#contributors)

## Description

Docker-compose setup for starting [Træfik](https://traefik.io/) with [Let's Encrypt](https://letsencrypt.org/).

## Setup

```sh
cd /opt
git clone https://github.com/solution-libre/docker-traefik.git traefik
cd traefik
```

Change domain and email values in `traefik.toml`.

Read this doc: [https://docs.traefik.io/user-guide/docker-and-lets-encrypt/](https://docs.traefik.io/user-guide/docker-and-lets-encrypt/)

## Usage

```sh
cd /opt/traefik
docker-compose up -d
```

## Development

[Solution Libre](https://www.solution-libre.fr)'s repositories are open projects, and community contributions are essential for keeping them great.


[Fork this repo on GitHub](https://github.com/solution-libre/docker-traefik/fork)

## Contributors

The list of contributors can be found at: https://github.com/solution-libre/docker-traefik/graphs/contributors
