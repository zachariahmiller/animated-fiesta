# 🏭 UDS Plane Package

##TODO##
Needs monitoring, redis (switch to valkey) with auth (vs no auth currently), fix minio connectivity, narrow down netpols more, add sso. 


[![Latest Release](https://img.shields.io/github/v/release/defenseunicorns/uds-package-plane)](https://github.com/defenseunicorns/uds-package-plane/releases)
[![Build Status](https://img.shields.io/github/actions/workflow/status/defenseunicorns/uds-package-plane/tag-and-release.yaml)](https://github.com/defenseunicorns/uds-package-plane/actions/workflows/tag-and-release.yaml)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/defenseunicorns/uds-package-plane/badge)](https://api.securityscorecards.dev/projects/github.com/defenseunicorns/uds-package-plane)

This package is designed for use as part of a bundle deployed on [UDS Core](https://github.com/defenseunicorns/uds-core).

## Prerequisites

Plane requires a postgres database, object storage and redis. Wiring plane to your dependencies is done primarily via helm values, which will require the use of a bundle created with uds-cli.

## Flavors

| Flavor | Description | Example Creation |
| ------ | ----------- | ---------------- |
| upstream | Uses upstream images within the package. | `zarf package create . -f upstream` |

## Releases

The released packages can be found in [ghcr](https://github.com/defenseunicorns/uds-package-plane/pkgs/container/packages%2Fuds%2Fplane).

## UDS Tasks (for local dev and CI)

*For local dev, this requires you install [uds-cli](https://github.com/defenseunicorns/uds-cli?tab=readme-ov-file#install)

> :white_check_mark: **Tip:** To get a list of tasks to run you can use `uds run --list`!

## Contributing

Please see the [CONTRIBUTING.md](./CONTRIBUTING.md)