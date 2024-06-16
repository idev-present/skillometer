# Reply Status List

### Метод: GET /dict/reply_status
#### Описание:
Этот метод предназначен для получения списка статусов откликов. Возвращает массив объектов, каждый из которых представляет собой статус отклика.

<api-endpoint openapi-path="../openapi.json" endpoint="/dict/reply_status" method="get">
<response type="200">
<sample>
[
  {
    "key": "NEW",
    "value": "Новый"
  },
  {
    "key": "CV_REVIEW",
    "value": "Проверка резюме"
  },
  {
    "key": "HR_INTERVIEW",
    "value": "Первичное интервью"
  },
  {
    "key": "CV_AGREEMENT",
    "value": "Выбор кандидата"
  },
  {
    "key": "JOB_INTERVIEW",
    "value": "Собеседование"
  },
  {
    "key": "REQUIRED_TASK",
    "value": "Техническое задание"
  },
  {
    "key": "WAITING",
    "value": "Принятие решения"
  },
  {
    "key": "OFFER_POSTED",
    "value": "Выставлен оффер"
  },
  {
    "key": "OFFER_ACCEPTED",
    "value": "Оффер принят"
  },
  {
    "key": "RESERVE",
    "value": "Резерв"
  },
  {
    "key": "DECLINED",
    "value": "Отказ"
  },
  {
    "key": "DONE",
    "value": "Готово"
  }
]
</sample>
</response>
</api-endpoint>