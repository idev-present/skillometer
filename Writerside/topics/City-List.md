# City List

### Метод: GET /dict/city
#### Описание:
Этот метод предназначен для получения списка городов. Возвращает массив объектов, каждый из которых представляет собой город.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/city" method="get">
<response type="200">
<sample>
[
    {
        "id": "kirov",
        "fias_id": "452a2ddf-88a1-4e35-8d8d-8635493768d4",
        "habr_id": 12,
        "habr_alias": "kirov",
        "name": "Киров",
        "country_name": "РФ",
        "region_name": "Кировская область"
    }
]
</sample>
</response>
</api-endpoint>