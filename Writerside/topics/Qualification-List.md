# Qualification List

### Метод: GET /dict/qualification
#### Описание:
Этот метод предназначен для получения списка квалификаций. Возвращает массив объектов, каждый из которых представляет собой квалификацию.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/qualification" method="get">
<response type="200">
<sample>
[
  {
    "id": "middle",
    "name": "Средний (Middle)",
    "habr_id": 4
  }
]
</sample>
</response>
</api-endpoint>