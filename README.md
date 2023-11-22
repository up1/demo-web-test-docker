# demo-web-test-docker


Run web
```
docker compose build web
docker compose up -d web
docker compose ps

docker compose down
```

Run test
```
docker compose build test
docker compose up test --build --remove-orphans --abort-on-container-exit 

docker compose down
```
