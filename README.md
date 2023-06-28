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