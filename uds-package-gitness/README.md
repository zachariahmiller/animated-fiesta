# Gitness UDS Package

## Blockers

[privileged docker in docker fun](https://github.com/harness/gitness/blob/8c18a93696ef9a7a4d6df5f8b767f5245045b587/charts/gitness/templates/deployment.yaml#L72)

- Requires EmptyDir on /tmp to create repos when running without exemptions. This is not extendible in the deployment.
- tries to reach out to docker need a way to override DOCKER_HOST or something
