# microservices - shop

Приложение для заказа товаров

# Использованные технологии

* Spring Boot – как основной фрэймворк
* MySQL – как основная реляционная база данных(Заказы и инвентарь(склад)).
* MongoDB - как нереляционная база данных(товары).
* testcontainers – для изолированного тестирования с базой данных
* Flyway – для ведения миграций схемы БД
* Maven – как система сборки приложения
* Lombok – для удобной работы с POJO классами
* KeyCloak - для идентификации и авторизации
* Kafka - для асинхронной отправки сообщений
* Grafana Stack - для мониторинга и наблюдаемости

# Код

RESTful приложение для заказа товаров.

* Обычная трёхслойная
  архитектура – Controller, Service, Repository
* Слой Repository реализован на JPA (Hibernate)
* Для стандартизированного описания RESTful API использовался openAPI
* Resilience4j для повышения отказоустойчивости


# Тесты

Написаны базовые с Testcontainers. Wiremock для тестов между сервисами

