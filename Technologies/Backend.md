Этот документ посвещён необходимым знаниям, относящихся к Java Backend, напрямую или косвенно.

## Общие знания

Владение общими знаниями хорошо тем, что они применимы к любой Backend платформе, будь то Java, .Net, NodeJS или другие.

### Клиент-серверное взаимодействие, IP адреса, DNS

Базовые идеи, о которых необходимо иметь общее представление. Что нужно знать:
- Что такое IP адрес
- Разница между TCP и UDP
- Что такое TCP сокет
- Клиент-серверное взаимодействие. Что именно происходит, когда браузер запрашивает страницу сайта
- Что такое DNS

Эти статьи помогут начать:
- https://developer.mozilla.org/ru/docs/Learn/Common_questions/How_does_the_Internet_work
- https://developer.mozilla.org/ru/docs/Learn/Getting_started_with_the_web/How_the_Web_works

### HTTP

Главный протокол WEB

Что нужно знать:
- HTTP методы
- Заголовки, cookies
- Коды ответа
- Form data, multipart form data

Поможет начать:
- https://ru.wikipedia.org/wiki/HTTP

## REST API

REST - набор правил взаимодействия клиента и сервера на основе HTTP. Сделать работающее клиент-серверное легко, элегантно его спроектировать - сложно. 

Что нужно знать:
- Отличие RESTful от RESTless
- Базовые дизайн принципы и типовые ошибки, которых следует избегать

Поможет начать:
- https://habr.com/ru/post/483202/
- https://habr.com/ru/post/351890/

Книга по дизайну REST API - https://www.amazon.com/REST-Design-Rulebook-Mark-Masse/dp/1449310508.

Проект #2 "обмен валют" содержит пример дизайна REST API.

## Java

Перейдём к знаниям, относящимся напрямую к Backend разработке на Java.

### Java Servlets

Сервлет - сущность в Java, реализующая клиент-серверное взаимодействие со стороны сервера. Сервлет принимает соединения от клиентов, и отвечает на запросы.

Что нужно уметь:
- Реализовывать сервлеты, пользуясь пакетом `javax.servlet-api`
- Запускать Java проект с сервлетами с помощью Tomcat

Поможет начать:
- https://www.baeldung.com/intro-to-servlets

### Spring Boot

### Шаблонизаторы веб страниц

## Что дальше

- Websocket
- Json vs Protobuf
- REST API vs GRPC
- GraphQL
- Micronaut, Quarkus
