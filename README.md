# Automated k6 load testing with Google Cloud CI/CD

This is an example repo for how to setup k6 with Google Cloud CI/CD to build load testing into an automation flow.

The full guide describing how to use this repository is located [here](https://k6.io/blog/integrating-k6-with-google-cloud-build/).

## Examples

| File                                                           | Description                                   |
| -------------------------------------------------------------- | --------------------------------------------- |
| [local-example/cloudbuild.yaml](local-example/cloudbuild.yaml) | Runs locally on Google's CI/CD infrastructure |
| [cloud-example/cloudbuild.yaml](cloud-example/cloudbuild.yaml) | Runs on k6 cloud                              |

## Run Local

```bash
# Run locally
k6 run scripts/test.js

# Run via Docker
docker run -i loadimpact/k6 run - <scripts/test.js

# Run via Docker Compose
docker-compose run k6
```
