# Backend

Этот документ посвящён необходимым знаниям, относящихся к Java Backend, напрямую или косвенно.

## Общие знания

Владение общими знаниями хорошо тем, что они применимы к любой Backend платформе, будь то Java, .Net, NodeJS или другие.

### Клиент-серверное взаимодействие, IP адреса, DNS

Базовые идеи, о которых необходимо иметь общее представление. Что нужно знать:
- Что такое IP адрес
- Разница между TCP и UDP
- Что такое TCP сокет
- Клиент-серверное взаимодействие. Что именно происходит, когда браузер запрашивает страницу сайта
- Что такое DNS

#### Избранные курсы и учебные ресурсы

- [https://developer.mozilla.org/ru/docs/Learn/Common_questions/How_does_the_Internet_work](https://developer.mozilla.org/ru/docs/Learn/Common_questions/How_does_the_Internet_work)
- [https://developer.mozilla.org/ru/docs/Learn/Getting_started_with_the_web/How_the_Web_works](https://developer.mozilla.org/ru/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

### HTTP

Главный протокол WEB

Что нужно знать:
- HTTP методы
- Заголовки, cookies
- Коды ответа
- Form data, multipart form data

#### Избранные курсы и учебные ресурсы

- [https://zametkinapolyah.ru/servera-i-protokoly/chto-nuzhno-znat-pro-http-protokol-veb-razrabotchiku-pravila-http-protokola.html](Статья) про HTTP простым языком
- Практика - проекты, начиная с 3

## REST API

REST - набор правил взаимодействия клиента и сервера на основе HTTP. Сделать работающее клиент-серверное легко, элегантно его спроектировать - сложно. 

Что нужно знать:
- Отличие RESTful от RESTless
- Базовые дизайн принципы и типовые ошибки, которых следует избегать

#### Избранные курсы и учебные ресурсы

- Статьи по REST на хабре - [#1](https://habr.com/ru/post/483202/), [#2](https://habr.com/ru/post/351890/)
- Книга по дизайну REST API - [https://www.amazon.com/REST-Design-Rulebook-Mark-Masse/dp/1449310508](https://www.amazon.com/REST-Design-Rulebook-Mark-Masse/dp/1449310508)
- Практика - проекты #3 ["Обмен валют"](../../Projects/CurrencyExchange/index.md) и #7 ["Планировщик задач"](../../Projects/TaskTracker/index.md) содержат примеры дизайна REST API

## Java

Перейдём к знаниям, относящимся напрямую к Backend разработке на Java.

### Java Servlets

Сервлет - сущность в Java, реализующая клиент-серверное взаимодействие со стороны сервера. Сервлет принимает соединения от клиентов, и отвечает на запросы.

Что нужно уметь:
- Реализовывать сервлеты, пользуясь пакетом `javax.servlet-api` (или `jakarta.servlet`)
- Запускать Java проект с сервлетами с помощью Tomcat

#### Избранные курсы и учебные ресурсы

- [Бесплатный курс](https://www.youtube.com/playlist?list=PLAma_mKffTOTTFqIkLXgHqVuL6xJhb0mr) по Java EE от Наиля Алиш
- [Статья](https://javarush.com/groups/posts/2529-chastjh-5-servletih-pishem-prostoe-veb-prilozhenie) с примерами на сайте Javarush
- [Краткое интро](https://www.baeldung.com/intro-to-servlets) в сервлеты от Baeldung
- Практика - проекты с 3 по 5

### Spring Boot

Spring Boot - основной фреймворк Java разработчика с долгой историей. Основная сложность - из-за возраста, у фреймворка существует несколько версий (Spring начинал свою историю как Spring Mvc), и одно и то же можно сделать несколькими способами, и новичку не всегда понятно, какой способ лучше.

Что нужно уметь:
- Работать с базами данных
- Реализовывать REST API
- Создавать веб страницы
- Библиотеки экосистемы Spring Boot - Spring Security, Spring Sessions

#### Избранные курсы и учебные ресурсы

- Начать можно с [бесплатного плейлиста](https://www.youtube.com/playlist?list=PLAma_mKffTOR5o0WNHnY0mTjKxnCgSXrZ) Алишева на YouTube
- [Spring - полный курс](https://swiftbook.org/courses/438) Наиля Алишева - разделы Spring Core, Spring MVC, Spring Boot, Spring Security
- Практика - проекты с 6 и 7

### Шаблонизаторы веб-страниц

Шаблонизатор - инструмент создания веб-страниц с динамическим контентом. Классический пример - отображение на веб-странице информации, прочитанной из базы данных.

Для Java и Spring существует множество шаблонизаторов. Остановимся на двух из них, JSP - старый, классический инструмент, который уже не используется, но на примере которого можно понять основные идеи шаблонизации. Thymeleaf - современный и мощный инструмент. 

Что нужно уметь:
- Передавать данные из Java в шаблон
- Thymyleaf - интеграция со Spring Boot, Thymeleaf фрагменты

#### Избранные курсы и учебные ресурсы

- [Видео](https://www.youtube.com/watch?v=w1FjeTZxQrQ&list=PLAma_mKffTOR5o0WNHnY0mTjKxnCgSXrZ&index=23) Алишева про Thymeleaf
- [Документация](https://www.thymeleaf.org/doc/tutorials/3.0/usingthymeleaf.html)
- Практика - проекты 5, 6

## Что дальше

Перечисленные выше знания и инструменты - база для Java Junior. Если есть желание и необходимость углубиться в Backend технологии, советую обратить внимание на:
- Websocket
- XML, Protobuf
- Альтернативны REST - SOAP, GRPC, GraphQL
- Более новые Java фреймворки - Micronaut, Quarkus
- Реактивный бэкенд - Spring Webflux
