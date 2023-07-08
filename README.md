# AQA_Java_Moscow_ITD
## microservices-demo

## Вот текст тестового задания:

1. Поднять контейнер из https://github.com/microservices-demo/microservices-demo

2. Написать на языке Java e2e тест по авторизации и добавления товара в корзину

3. Проверить что сумма цены товаров в корзине соответствует сумме цен заказанных товаров

## Выполнение
### 1. Развертывание приложения с помощью Docker Compose
Это руководство описывает процесс развертывания и запуска приложения с помощью инструмента Docker Compose.
#### Предварительные требования
* Docker и Docker Compose должны быть установлены на вашем компьютере и запущен.
#### Шаги
* Скачайте исходный код с репозитория GitHub:
```
git clone https://github.com/microservices-demo/microservices-demo.git
```
* Перейдите в каталог `deploy/docker-compose`:
```
cd microservices-demo/deploy/docker-compose
```
* Соберать все Docker-образы микросервисов командой:
```sh
docker-compose build
или
docker-compose build --no-cache
```
* Запустите приложение с помощью команды:
```sh
docker-compose up -d
```
* Для того, чтобы узнать порты, можно выполнить команду:
```sh
docker-compose ps
```
* После того как приложение будет запущено, откройте веб-браузер и перейдите на страницу `http://localhost:80`. Откроется веб-интерфейс приложения.

* Чтобы остановить приложение, выполните команду:
```sh
docker-compose down
```

### 2. Написать на языке Java e2e тест по авторизации и добавления товара в корзину
    и
### 3. Проверить что сумма цены товаров в корзине соответствует сумме цен заказанных товаров
    объединим задание в корнетпроекта папке srs

#### Описание использовал следующее:
    Java 17
    gradle
    playwright
    JUnit 5
    Allure

