# Задание 2: REST API
## Пример запроса

```http
GET /api/v1/retail?city=spb&limit=20
Host: api.petrushka-zelenaya.ru
Authorization: Bearer <token>
Accept: application/json
```

## Пример ответа

```{
  "title": "Выберите магазин",
  "shops": [
    {
      "id": "metro_1",
      "name": "METRO",
      "logo_url": "https://petrushka.ru/images/shops/metro.png",
      "delivery_time": {
        "type": "slot",
        "label": "сегодня 21:00–23:00",
        "from": "2026-02-10T21:00:00+03:00",
        "to": "2026-02-10T23:00:00+03:00"
      },
      "external_url": "https://metro-cc.ru/",
      "is_active": true
    },
    {
      "id": "ashan_1",
      "name": "Ашан",
      "logo_url": "https://petrushka.ru/images/shops/ashan.png",
      "delivery_time": {
        "type": "slot",
        "label": "сегодня 18:00–20:00",
        "from": "2026-02-10T18:00:00+03:00",
        "to": "2026-02-10T20:00:00+03:00"
      },
      "external_url": "https://www.auchan.ru",
      "is_active": true
    },
    {
      "id": "vkusvill_1",
      "name": "ВкусаВилл",
      "logo_url": "https://petrushka.ru/images/shops/vkusvill.png",
      "delivery_time": {
        "type": "minutes",
        "label": "от 20 до 60 минут",
        "min_minutes": 20,
        "max_minutes": 60
      },
      "external_url": "https://vkusvill.ru/",
      "is_active": true
    },
    {
      "id": "victoria-group_1",
      "name": "Виктория",
      "logo_url": "https://petrushka.ru/images/shops/victoria-group.png",
      "delivery_time": {
        "type": "slot",
        "label": "сегодня 17:00–19:00",
        "from": "2026-02-10T17:00:00+03:00",
        "to": "2026-02-10T19:00:00+03:00"
      },
      "external_url": "https://victoria-group.ru/",
      "is_active": true
    }
  ]
}
```
