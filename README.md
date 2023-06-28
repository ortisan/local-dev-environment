# Stack Local Dev

Project with integration tests environment.

## Starting project


```sh
docker-compose up -d
```

## Testing

```sh
curl --location --request GET 'http://localhost:1080/assets/indices' \
--header 'Content-Type: application/json'
```