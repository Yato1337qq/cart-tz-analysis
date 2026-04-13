# Задание 2: Проектирование API

## 📌 Описание

API возвращает список магазинов-партнёров для отображения на экране выбора магазина.

---

## 📥 Запрос

GET /api/v1/partners

---

## 📤 Ответ

```json
{
  "partners": [
    {
      "id": 1,
      "name": "METRO",
      "logoUrl": "https://example.com/metro.png",
      "deliveryType": "interval",
      "delivery": {
        "from": "21:00",
        "to": "23:00"
      },
      "link": "https://metro.ru"
    },
    {
      "id": 2,
      "name": "Ашан",
      "logoUrl": "https://example.com/auchan.png",
      "deliveryType": "interval",
      "delivery": {
        "from": "18:00",
        "to": "20:00"
      },
      "link": "https://auchan.ru"
    },
    {
      "id": 3,
      "name": "ВкусВилл",
      "logoUrl": "https://example.com/vkusvill.png",
      "deliveryType": "fast",
      "delivery": {
        "minMinutes": 20,
        "maxMinutes": 60
      },
      "link": "https://vkusvill.ru"
    }
  ]
}
