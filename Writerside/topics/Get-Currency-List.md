# Get Currency List

### Метод: GET /dict/currency
#### Описание:
Этот метод предназначен для получения списка валют. Возвращает массив объектов, каждый из которых представляет собой валюту и ее ключевое значение.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/currency" method="get">
<response type="200">
<sample>
[
  {
    "key": "RUR",
    "value": "₽"
  }
]
</sample>
</response>
</api-endpoint>
