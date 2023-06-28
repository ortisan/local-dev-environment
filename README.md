# Stack Local Dev

Project with integration tests environment.

[![release-please](https://github.com/ortisan/local-dev-environment/actions/workflows/release-please.yml/badge.svg?branch=main)](https://github.com/ortisan/local-dev-environment/actions/workflows/release-please.yml)

## Starting project


```sh
docker-compose up -d
```

## Testing

```sh
curl --location --request GET 'http://localhost:1080/assets/indices' \
--header 'Content-Type: application/json'
```

## Running Sonar

```sh
export SONARQUBE_URL=http://host.docker.internal:9000
export SONAR_LOGIN=squ_fde11c23678cfd9c6a154e9019081b517d6fde0f
docker run \
--rm \
-e SONAR_HOST_URL="http://host.docker.internal:9000" \
-e SONAR_LOGIN="squ_fde11c23678cfd9c6a154e9019081b517d6fde0f" \
-v "$(pwd)/golang-example:/usr/src" \
sonarsource/sonar-scanner-cli
```