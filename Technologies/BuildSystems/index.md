# Системы сборки

Документ посвещён необходимым знаниям, относящимся к системам сборки Java проектов - Maven и Gradle.

Первой популярной сборки для Java был Apache Ant, но он морально устарел и на практике почти не встречается.

Начинать знакомство с системами сборки предлагаю с Maven, практиковаться с ним на проектах до пятого включительно, в проектах 6 и 7 попробовать Gradle. Maven появился раньше, поэтому, логичнее начинать с него, потом переключиться на Gradle.

На уровне Junior, принципиальной разницы между двумя этими инструментами нет, в работе можно встретить обе системы сборки, поэтому есть смысл попрактиковаться с обеими.

## Maven

Для изучения Maven нет необходимости читать целые книги или проходить курсы. Начать стоит с краткой выжимки основных идей (например - https://habr.com/ru/post/77382/), далее, немного углубиться в теорию и заняться практикой.

Что нужно знать, где почитать:

- Идеи Maven - что такое Maven lifecycle, phase и goal - [https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html)
- Локальный репозиторий Maven - [https://www.baeldung.com/maven-local-repository](https://www.baeldung.com/maven-local-repository)
- Maven POM - что это такое, основные секции файла - зависимости, build плагины, свойства проекта - [https://maven.apache.org/guides/introduction/introduction-to-the-pom.html](https://maven.apache.org/guides/introduction/introduction-to-the-pom.html)
- Практика - создание Spring Boot Maven проекта с помощью Spring Initializr:
  - На сайте [https://start.spring.io/](https://start.spring.io/)
  - В среде Intellij IDEA
- Практика - использование Maven в Java проектах
  - Добавление зависимостей
  - Сборка и запуск приложения через командную строку

Полезно, но не обязательно:

- Что такое Maven BOM - [https://www.baeldung.com/spring-maven-bom](https://www.baeldung.com/spring-maven-bom)
- Что такое транзитивные зависимости, и как Maven BOM решает эту проблему - [https://reflectoring.io/maven-bom/](https://reflectoring.io/maven-bom/)
- Maven BOM фреймворка Spring Boot - [https://www.baeldung.com/spring-maven-bom](https://www.baeldung.com/spring-maven-bom)
- Multi-module проекты - [https://www.baeldung.com/maven-multi-module](https://www.baeldung.com/maven-multi-module)
- Maven архетипы - [https://www.baeldung.com/maven-archetype](https://www.baeldung.com/maven-archetype)
- Развёртывание своих Maven репозиториев
- Релиз артефактов в Maven репозитории

## Gradle

Gradle - более новая система сборки, чем Maven. Для Java Backend проектов на Spring, Maven и Gradle в большинстве случаев взаимозаменяемы, лично я предпочитаю Gradle из-за производительности. Для Android проектов используется только Gradle.

Что нужно знать, где почитать:

- Отличия Gradle от Maven - [https://gradle.org/maven-vs-gradle/](https://gradle.org/maven-vs-gradle/)
- Gradle Lifecycle - [https://docs.gradle.org/current/userguide/build_lifecycle.html](https://docs.gradle.org/current/userguide/build_lifecycle.html)
- Что такое DSL. Gradle Groovy/Kotlin DSL - [https://docs.gradle.org/current/userguide/tutorial_using_tasks.html](https://docs.gradle.org/current/userguide/tutorial_using_tasks.html)
- Практика - создание Spring Boot Gradle проекта с помощью Spring Initializr:
  - На сайте [https://start.spring.io/](https://start.spring.io/)
  - В среде Intellij IDEA
- Практика - использование Gradle в Java проектах
  - Добавление зависимостей
  - Сборка и запуск приложения через командную строку
