# Insnotify

Приложение для интеграции с InSales и Mark для функционала "Сообщить о поступлении".

## Описание

Insnotify - это партнерское приложение, которое интегрируется с InSales и Mark для предоставления функционала уведомлений о поступлении товаров в наличии.

## Требования

* Ruby 3.4.7
* PostgreSQL 15
* Rails 8.1.1

## Установка

1. Установите зависимости:
```bash
bundle install
```

2. Создайте базу данных:
```bash
bin/rails db:create
bin/rails db:migrate
```

3. Настройте credentials:
```bash
EDITOR="code --wait" bin/rails credentials:edit
```

## Развертывание

Приложение развертывается через Kamal:
```bash
bin/kamal deploy
```

## Интеграция

- **InSales**: Установка через `/insales/install`
- **Mark**: Интеграция через `/insnotify/install` и `/insnotify/autologin`
