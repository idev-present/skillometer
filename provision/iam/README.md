# IAM

[Doc](https://casdoor.org/)

### Install
#### Create database
```postgresql
CREATE USER iam_dba WITH ENCRYPTED PASSWORD 'iam_dba_idev2512';
CREATE DATABASE iam_db;
GRANT ALL PRIVILEGES ON DATABASE iam_db TO iam_dba;
```

```shell
helm upgrade --install --namespace skillometer --values=clusters/skillometer/iam/values.yaml casdoor oci://registry-1.docker.io/casbin/casdoor-helm-charts --version v1.629.0
```