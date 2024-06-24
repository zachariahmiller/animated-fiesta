# 🏭 UDS Nats Package

[![Latest Release](https://img.shields.io/github/v/release/defenseunicorns/uds-package-nats)](https://github.com/defenseunicorns/uds-package-nats/releases)
[![Build Status](https://img.shields.io/github/actions/workflow/status/defenseunicorns/uds-package-nats/tag-and-release.yaml)](https://github.com/defenseunicorns/uds-package-nats/actions/workflows/tag-and-release.yaml)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/defenseunicorns/uds-package-nats/badge)](https://api.securityscorecards.dev/projects/github.com/defenseunicorns/uds-package-nats)

This package is designed for use as part of a bundle deployed on [UDS Core](https://github.com/defenseunicorns/uds-core).

## Prerequisites

Nats requires a postgres database. Wiring coder to your dependencies is done primarily via helm values, which will require the use of a bundle created with uds-cli.

## Flavors

| Flavor | Description | Example Creation |
| ------ | ----------- | ---------------- |
| upstream | Uses upstream images within the package. | `zarf package create . -f upstream` |

## Releases

The released packages can be found in [ghcr](https://github.com/defenseunicorns/uds-package-nats/pkgs/container/packages%2Fuds%2Fnats).

## UDS Tasks (for local dev and CI)

*For local dev, this requires you install [uds-cli](https://github.com/defenseunicorns/uds-cli?tab=readme-ov-file#install)

> :white_check_mark: **Tip:** To get a list of tasks to run you can use `uds run --list`!

## Contributing

Please see the [CONTRIBUTING.md](./CONTRIBUTING.md)