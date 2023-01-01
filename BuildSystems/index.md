# Системы сборки

Документ посвещён необходимым знаниям, относящихся к системам сборки Java проектов - Maven и Gradle.

Первой системой сборки для Java был Apache Ant, но он уже морально устарел и на практике почти не встречается.

Начинать знакомство с системами сборки предлагаю с Maven, практиковаться с ним на проектах до пятого включительно, в проектах 6 и 7 попробовать Gradle. С Maven начать проще, потому что он появился раньше, и, зная Maven, понять Gradle будет проще.

На уровне Junior, принципиальной разницы между двумя этими инструментами нет, в работе можно встретить обе системы сборки, поэтому есть смысл попрактиковаться с обеими.

## Maven

Для изучения Maven нет необходимость читать целые книги или проходить курсы. Начать стоит с краткой выжимки основных идей (например - https://habr.com/ru/post/77382/), далее, немного углубиться в теорию и заняться практикой.

Что нужно знать, где почитать:

- Идеи Maven - что такое Maven lifecycle, phase и goal - https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html
- Maven POM - что это такое, основные секции файла - зависимости, build плагины, свойства проекта - https://maven.apache.org/guides/introduction/introduction-to-the-pom.html
- Практика - создание Spring Boot Maven проекта с помощью Spring Initializr:
  - На сайте https://start.spring.io/
  - В среде Intellij IDEA
- Практика - использование Maven в Java проектах
  - Добавление зависимостей
  - Сборка и запуск приложения через командную строку

Полезно, но не обязательно:

- Что такое Maven BOM - https://www.baeldung.com/spring-maven-bom
- Что такое транзитивные зависимости, и как Maven BOM решает эту проблему - https://reflectoring.io/maven-bom/
- Maven BOM фреймворка Spring Boot - https://www.baeldung.com/spring-maven-bom
- Multi module проекты - https://www.baeldung.com/maven-multi-module
- Maven архетипы - https://www.baeldung.com/maven-archetype

## Gradle

Gradle - более новая система сборки чем Maven. Для Java Backend проектов на Spring, Maven и Gradle взаимозаменяемы в большинстве случаев. Для Android проектов используется только Gradle.

Что нужно знать, где почитать:

- Отличия Gradle от Maven - https://gradle.org/maven-vs-gradle/
- Gradle Lifecycle - https://docs.gradle.org/current/userguide/build_lifecycle.html
- Что такое DSL. Gradle Groovy/Kotlin DSL - https://docs.gradle.org/current/userguide/tutorial_using_tasks.html
- Практика - создание Spring Boot Gradle проекта с помощью Spring Initializr:
  - На сайте https://start.spring.io/
  - В среде Intellij IDEA
- Практика - использование Gradle в Java проектах
  - Добавление зависимостей
  - Сборка и запуск приложения через командную строку
