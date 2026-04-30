# Desc Service

Сервис управления категориями и темами.

## 🔧 Технологии
- Java 21
- Spring Boot 2.7.11
- Spring Security + OAuth2
- PostgreSQL
- Liquibase
- Eureka Client

## 📦 Порт
9902

## 🗄️ База данных
- Имя: cd_desc
- Пользователь: postgres
- Пароль: password

## 📚 API Endpoints

| Метод | URL | Описание |
|-------|-----|----------|
| GET | /categories/ | Список категорий |
| GET | /categories/most_pop | Популярные категории |
| GET | /topics/{id} | Темы категории |
| GET | /topic/{id} | Просмотр темы |
| GET | /category/ping | Проверка работы |
| POST | /category/ | Создать категорию (ADMIN) |
| PUT | /category/ | Обновить категорию (ADMIN) |
| DELETE | /category/{id} | Удалить категорию (ADMIN) |
| POST | /topic/ | Создать тему (ADMIN) |
| PUT | /topic/ | Обновить тему (ADMIN) |
| DELETE | /topic/ | Удалить тему (ADMIN) |

## 📄 Swagger
http://localhost:9902/swagger-ui/index.html

## 🔗 Eureka
Регистрируется под именем desc

## 🚀 Запуск
```bash
mvn spring-boot:run