# Cachet for OpenShift 3

## Description
Templates and imagestreams that add Cachet to your OpenShift cluster.

Tested for OpenShift 3.6 and 3.7.

## Quickstart
1. Add official imagestream to OpenShift.
```shell
oc create -f imagestreams/cachet-official.yaml
```
2. Add template to OpenShift.
```
oc create -f templates/cachet.yaml
```
3. Deploy template using WebUI or CLI.
```
oc process templates/cachet DB_USERNAME=user \
                            DB_PASSWORD=passwd \
                            DB_HOST=mysql.host.com \
                            DB_DATABASE=sampledb \
                            DB_PORT=3306 \
                            DB_DRIVER=mysql \
                            CACHET_URL=cachet.domain.com | \
oc create -f -
```
4. Setup Cachet using Cachet WebUI.
5. ...
6. Profit.
