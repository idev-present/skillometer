# Search Status List

### Метод: GET /dict/search_status
#### Описание:
Этот метод предназначен для получения списка статусов резюме соискателей. Возвращает массив объектов, каждый из которых представляет собой статус поиска работы.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/search_status" method="get">
<response type="200">
<sample>
[
  {
    "id": "active",
    "name": "В активном поиске",
    "habr_id": null
  },
  {
    "id": "not_active",
    "name": "Не ищу работу",
    "habr_id": null
  },
  {
    "id": "passive",
    "name": "Рассмотрю предложения",
    "habr_id": null
  }
]
</sample>
</response>
</api-endpoint>