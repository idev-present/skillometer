# Employment Type List

### Метод: GET /dict/employment_type
#### Описание:
Этот метод предназначен для получения списка типов занятости. Возвращает массив объектов, каждый из которых представляет собой тип занятости.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/employment_type" method="get">
<response type="200">
<sample>
[
  {
    "id": "full_time",
    "name": "Полная занятость",
    "habr_id": "1",
    "hh_id": "1"
  },
  {
    "id": "part_time",
    "name": "Частичная занятость",
    "habr_id": "2",
    "hh_id": "2"
  }
]
</sample>
</response>
</api-endpoint>