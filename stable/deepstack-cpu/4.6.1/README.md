# deepstack-cpu

![Version: 4.6.0](https://img.shields.io/badge/Version-4.6.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: auto](https://img.shields.io/badge/AppVersion-auto-informational?style=flat-square)

DeepStack AI provides AI features including Face Recognition, Object Detection, Scene Recognition and custom AI Models

**Homepage:** <https://github.com/truecharts/apps/tree/master/charts/stable/deepstack-cpu>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| TrueCharts | info@truecharts.org | truecharts.org |
| stavros-k | stavros-k@users.noreply.github.com | truecharts.org |

## Source Code

* <https://github.com/johnolafenwa/DeepStack>
* <https://hub.docker.com/r/deepquestai/deepstack>
* <https://www.deepstack.cc/>

## Requirements

Kubernetes: `>=1.16.0-0`

| Repository | Name | Version |
|------------|------|---------|
| https://truecharts.org/ | common | 6.8.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| env.MODE | string | `"High"` |  |
| env.MODELSTORE-DETECTION | string | `"/modelstore/detection"` |  |
| env.PGID | string | `"568"` |  |
| env.PUID | string | `"568"` |  |
| env.VISION-DETECTION | string | `"True"` |  |
| env.VISION-FACE | string | `"True"` |  |
| env.VISION-SCENE | string | `"True"` |  |
| envTpl.GROUP_ID | string | `"{{ .Values.env.PGID }}"` |  |
| envTpl.USER_ID | string | `"{{ .Values.env.PUID }}"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"deepquestai/deepstack"` |  |
| image.tag | string | `"cpu-2021.02.1"` |  |
| persistence.config.enabled | bool | `true` |  |
| persistence.config.mountPath | string | `"/datastore"` |  |
| persistence.config.type | string | `"emptyDir"` |  |
| service.main.enabled | bool | `true` |  |
| service.main.ports.main.port | int | `5000` |  |
| strategy.type | string | `"Recreate"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)