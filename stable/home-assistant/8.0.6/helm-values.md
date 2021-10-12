# Default Helm-Values

TrueCharts is primarily build to supply TrueNAS SCALE Apps.
However, we also supply all Apps as standard Helm-Charts. In this document we aim to document the default values in our values.yaml file.

Most of our Apps also consume our "common" Helm Chart.
If this is the case, this means that all values.yaml values are set to the common chart values.yaml by default. This values.yaml file will only contain values that deviate from the common chart.
You will, however, be able to use all values referenced in the common chart here, besides the values listed in this document.

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| env | object | `{}` |  |
| git.deployKey | string | `""` |  |
| git.deployKeyBase64 | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/truecharts/home-assistant"` |  |
| image.tag | string | `"v2021.10.3@sha256:ddc4b06d0712263614bd4a2e05cd65fdc2f710ffce4ed0a1ab59ed62361fde5a"` |  |
| influxdb.architecture | string | `"standalone"` |  |
| influxdb.authEnabled | bool | `false` |  |
| influxdb.database | string | `"home_assistant"` |  |
| influxdb.enabled | bool | `false` |  |
| influxdb.persistence.enabled | bool | `false` |  |
| persistence.config.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.config.enabled | bool | `true` |  |
| persistence.config.mountPath | string | `"/config"` |  |
| persistence.config.size | string | `"100Gi"` |  |
| persistence.config.type | string | `"pvc"` |  |
| persistence.varrun.enabled | bool | `true` |  |
| postgresql.enabled | bool | `false` |  |
| postgresql.persistence.enabled | bool | `false` |  |
| postgresql.postgresqlDatabase | string | `"home-assistant"` |  |
| postgresql.postgresqlPassword | string | `"home-assistant-pass"` |  |
| postgresql.postgresqlUsername | string | `"home-assistant"` |  |
| prometheus.serviceMonitor.enabled | bool | `false` |  |
| service.main.ports.main.port | int | `8123` |  |

All Rights Reserved - The TrueCharts Project