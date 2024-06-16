# Skillometer

![made_by](https://img.shields.io/badge/made_by-IDEV-0d9488.svg?style=flat-square)

## Documentation

- [Documentation](https://idev-present.github.io/skillometer)
- [Project management](https://github.com/orgs/idev-present/projects/1/views/1)


## Demo
- [Documentation](https://idev-present.github.io/skillometer)
- [API](https://skillometer.idev-present.com/api/v1/docs)
- [WEB+TWA](https://skillometer.idev-present.com/)
- [WEB admin](https://admin.skillometer.idev-present.com/)
- 
## Demo accounts
Search in [Documentation](https://idev-present.github.io/skillometer/user-manual.html)



## Source code repository

- [root](https://github.com/idev-present/skillometer) - Navigation & Provision & Documentation
- [API](https://github.com/idev-present/skillometer-api)
- [WEB admin](https://github.com/idev-present/skillometer-web-admin)
- [WEB+TWA](https://github.com/idev-present/skillometer-app-client)

## Artefacts
- [spec.md](artefacts/input/spec.md)
- [use cases](artefacts/input/cases)
- [C4 context](artefacts/architecture/C4/C4_context.puml)
- [C4_containers](artefacts/architecture/C4/C4_containers.puml)
- [status flow](artefacts/architecture/status_scheme.puml)
- [DB schema](artefacts/architecture/DB_schema.puml)

### External support system
- Cloud.ru - kubernetes cluster
- Traefik - reverse proxy
- Casdoor - Identity & Access Manager

## Contribution Setup
1. Setup kubernetes cluster (master+node, ip loadbalancer, disks, buckets)
2. Setup proxy + ssl certs (+setup cloudflare to generate letsencrypt wildcard certificates). Flow `provision/proxy/README.md`
3. Setup postgres database (+persistence volume) Flow `provision/postgres/README.md`
4. Setup IAM (+create database for iam) Flow `provision/iam/README.md`
   1. Create organization
   2. Create application
   3. Setup SMTP config
   4. Integrate clients to IAM
5. Setup projects
   1. API. Flow `api/README.md`
   2. WEB admin. Flow `admin/README.md`
   3. Client. Flow `client/README.md`

## Authors

| Name             | Контакты                                 |
|------------------|------------------------------------------|
| Журавлев Илья    | [telegram](https://t.me/ichiro18)        |
| Журавлев Игорь   | [telegram](https://t.me/NeOMBouncer)     |
| Катаргин Кирилл  | [telegram](https://t.me/kirill_katargin) |
| Арасланов Максим | [telegram](https://t.me/MaxAraslanov)    |
| Кротов Илья      | [telegram](https://t.me/Ilya_Krotov043)  |