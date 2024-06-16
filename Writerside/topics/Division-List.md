# Division List

### Метод: GET /dict/division
#### Описание:
Этот метод предназначен для получения списка специализаций. Возвращает массив объектов, каждый из которых представляет собой подразделение.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/division" method="get">
<response type="200">
<sample>
[
  {
    "id": "frontend_developer",
    "name": "Фронтенд разработчик",
    "habr_id": 3
  }
]
</sample>
</response>
</api-endpoint>