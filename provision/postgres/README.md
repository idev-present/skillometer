# Postgres

### Install
```shell
helm upgrade --install --namespace skillometer --values=clusters/skillometer/postgres/values.yaml postgres oci://registry-1.docker.io/bitnamicharts/postgresql
```