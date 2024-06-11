# C4 Context

Уровень контекста служит для предоставления общей картины системы и ее окружения. Основная цель этого этапа – дать представление о том, как система взаимодействует с внешним миром и кто ее основные пользователи.

## Glossary

Список определений или глоссарий:

Person
: Участник системы имеюший доступ к админскому приложению

System
: Админское приложение.

External Person
: Участник системы имеющий доступ к клиентскому приложению.

External System
: Внешние системы.

## Схема
```plantuml
@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml
' uncomment the following line and comment the first to use locally
' !include C4_Context.puml

LAYOUT_WITH_LEGEND()

title C4 Context системы "Skillometer"

Person(customer, "Рекрутер", "Пользователь системы с персональным аккаунтом.")
Person_Ext(user, "Соискатель", "Пользователь Телеграм.")
System(skillometer_system, "Системы Skillometer", "Система позволяющее работать с актуальными вакансиями и резюме соискателей")

System_Ext(smtp, "SMTP", "Служит для отправки уведомлений участввующим лицам процесса")
System_Ext(telegram, "Telegram", "Система задействована как клиентское приложение")
System_Ext(google, "Google Календарь", "Сервис планирования и организации времени, который используется для управления рабочим графиком рекрутера и назначения встреч с соискателями")
System_Ext(habr, "Habr карьера", "Система из которой получаем акьуальные вакансии")
System_Ext(headhunter, "HeadHunter", "Система из которой получаем акьуальные вакансии")
System_Ext(reksoft, "Reksoft", "ATS система, система из которой получаем акьуальные вакансии, в далнейше как админское приложение")
System_Ext(gpt, "чат GPT", "ИИ для помощи в редактировании резюме")
System_Ext(s3, "Хранилище S3", "Система изпользуемая для хранения документов (резюме)")
System_Ext(google_meat, "Google Meat", "Конференция для проведения собеседований")

Rel(customer, skillometer_system, "Использует")
Rel_Back(customer, smtp, "Отправляет e-mails на")
Rel_Back(user, smtp, "Sends e-mails to")
Rel_Neighbor(skillometer_system, smtp, "Отправляет e-mails на")
BiRel(skillometer_system, telegram, "Обмен данными")
Rel(user, telegram, "Использует")
Rel_Back(user, telegram, "Отображает информацию")
Rel(skillometer_system, habr, "Актуализация вакансий")
Rel(skillometer_system, headhunter, "Актуализация вакансий")
Rel(skillometer_system, reksoft, "Актуализация вакансий")
Rel(skillometer_system, google, "Записи в календаре")
BiRel(skillometer_system, gpt, "Рерайт резюме")
BiRel(skillometer_system, s3, "Обмен файлами")
BiRel(skillometer_system, google_meat, "Создание конференции")
@enduml
```
