# Импорт тестовых баз данных MySQL

В этом наборе находятся стандартные демонстрационные базы данных MySQL:

- **sakila** — база данных для работы с видеопрокатом (фильмы, актёры, аренда).
- **employees** — база сотрудников (демонстрация работы с HR-данными).
- **world** — база стран, городов и языков.
- **cars** — база данных розничного магазина масштабных моделей классических автомобилей.  
  Содержит типичные бизнес-данные: информацию о клиентах, товарах, заказах, позициях заказов и многое другое.

## Требования

- Установленный MySQL Server
- Создать пользователя с правами администратора и удаленного доступа.

## Подготовка

Скачайте репозиторий через команду :

> git clone https://gitlab.irkat.ru/Bpeg/db-education.git

## Импорт в MySQL вручную

### Через командную строку

```bash
# world
mysql < database-dumps/world/world.sql

# employees
mysql < database-dumps/employees/employees.sql

# sakila
mysql < database-dumps/sakila/sakila-schema.sql
mysql -u root -p < database-dumps/sakila/sakila-data.sql

# cars 
mysql < database-dumps/cars/cars.sql
