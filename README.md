# Workshop with Docker
* Web with ReactJS
* Testing
  * UI Testing with Playwright
  * UI Testing with Robot framework and selenium
  * API Testing with Postman and newman
* [Scale Appium and Selenium](https://github.com/up1/docker-appium-selenium-grid)
  * https://www.somkiat.cc/selinium-grid-4-and-appium/


## Run web
```
docker compose build web
docker compose up -d web
docker compose ps

docker compose down
```

## Run UI Testing with Playwright
```
docker compose build test
docker compose up test --build --remove-orphans --abort-on-container-exit 
```

## Run UI Testing with Robot framework and selenium
```
docker compose build robot
docker compose up robot --build --remove-orphans --abort-on-container-exit 
```

## Run API Testing with Postman and newman
```
docker compose build api_test
docker compose up api_test --build --remove-orphans --abort-on-container-exit 
```
