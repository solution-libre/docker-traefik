# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- markdownlint-configure-file { "MD024": { "allow_different_nesting": true } } -->

## [1.3.0] 2021-03-05

### Added

- Enable HTTPs compression.

## [1.2.0] 2021-03-04

### Added

- Add `ACME_EMAIL`and `DOCKER_DOMAIN` environment variables.
- Add Github Actions for check.

### Fixed

- Fix Traefik option syntax.

### Security

- Improved HTTPs security.

## [1.1.0] 2018-11-23

### Changed

- Upgrade to [Træfik](https://traefik.io/) [v1.7](https://doc.traefik.io/traefik/v1.7/).

## [1.0.0] 2018-04-10

### Added

- [Docker Compose](https://docs.docker.com/compose/) setup for starting [Træfik](https://traefik.io/)
[v1.6](https://doc.traefik.io/traefik/v1.6/) with [Let's Encrypt](https://letsencrypt.org/).

[1.3.0]: https://github.com/solution-libre/docker-traefik/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/solution-libre/docker-traefik/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/solution-libre/docker-traefik/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/solution-libre/docker-traefik/releases/tag/v1.0.0
