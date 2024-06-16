# Skill List

### Метод: GET /dict/skill
#### Описание:
Этот метод предназначен для получения списка навыков. Возвращает массив объектов, каждый из которых представляет собой навык.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/skill" method="get">
<response type="200">
<sample>
[
  {
    "id": "typescript",
    "name": "TypeScript",
    "type": "hard",
    "qualification_id": null,
    "division_id": "frontend_razrabotchik",
    "habr_id": 245
  },
]
</sample>
</response>
</api-endpoint>