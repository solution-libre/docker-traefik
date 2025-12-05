# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- markdownlint-configure-file { "MD024": { "siblings_only": true } } -->

## [3.1.0] - 2025-12-05

### Added

- Environment variable `NETWORK_NAME` to configure external network name (default: `web`)

## [3.0.0] - 2025-01-06

### Changed

- Upgrade to [Traefik](https://traefik.io/) [v3.3](https://doc.traefik.io/traefik/v3.3/)
- Use environment variables instead of CLI options
- Convert TOML file to YAML
- Remove unsecure Chipers:
  - TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA
  - TLS_RSA_WITH_AES_256_GCM_SHA384
  - TLS_RSA_WITH_AES_256_CBC_SHA

## [2.2.0] - 2024-06-01

### Added

- Environment variable `VERSION` to set Traefik version
- CLI option to enable the Prometheus metrics

### Changed

- Upgrade to [Traefik](https://traefik.io/) [v2.11](https://doc.traefik.io/traefik/v2.11/).
- Rename the `docker-volumes` file to `volumes`

## [2.1.0] - 2023-08-23

### Changed

- Upgrade to [Traefik](https://traefik.io/) [v2.10](https://doc.traefik.io/traefik/v2.10/).
- Rename the `docker-compose.yml` file to `compose.yaml`

## [2.0.0] - 2022-07-15

### Added

- Add a default middleware to:
  - Force Strict-Transport-Security,
  - Force X-XSS-Protection,
  - Force X-Content-Type-Options: nosniff.
- Add [Dependabot](https://github.com/dependabot) in CI.

### Changed

- Upgrade to [Traefik](https://traefik.io/) [v2.8](https://doc.traefik.io/traefik/v2.8/).
- Set minimum version of TLS to v1.2.
- Move acme.json to a named volume.

## [1.3.0] - 2021-03-05

### Added

- Enable HTTPs compression.

## [1.2.0] - 2021-03-04

### Added

- Add `ACME_EMAIL`and `DOCKER_DOMAIN` environment variables.
- Add Github Actions for check.

### Fixed

- Fix Traefik option syntax.

### Security

- Improved HTTPs security.

## [1.1.0] - 2018-11-23

### Changed

- Upgrade to [Traefik](https://traefik.io/) [v1.7](https://doc.traefik.io/traefik/v1.7/).

## [1.0.0] - 2018-04-10

### Added

- [Docker Compose](https://docs.docker.com/compose/) setup for starting [Traefik](https://traefik.io/)
[v1.6](https://doc.traefik.io/traefik/v1.6/) with [Let's Encrypt](https://letsencrypt.org/).

[3.1.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v3.0.0...v3.1.0
[3.0.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v2.2.0...v3.0.0
[2.2.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v2.1.0...v2.2.0
[2.1.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v2.0.0...v2.1.0
[2.0.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v1.3.0...v2.0.0
[1.3.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v1.2.0...v1.3.0
[1.2.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v1.1.0...v1.2.0
[1.1.0]: https://usine.solution-libre.fr/docker/traefik/-/compare/v1.0.0...v1.1.0
[1.0.0]: https://usine.solution-libre.fr/docker/traefik/-/releases/v1.0.0
