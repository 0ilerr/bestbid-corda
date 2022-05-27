# bestbid-api-corda

![Version: 0.0.1](https://img.shields.io/badge/Version-0.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: bestbid-api-corda-v0.0.1-SNAPSHOT](https://img.shields.io/badge/AppVersion-bestbid--api--corda--v0.0.1--SNAPSHOT-informational?style=flat-square)

A Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| containerPort | int | `8080` |  |
| fullnameOverride | string | `""` |  |
| healthcheck.livenessProbe.httpGet.path | string | `"/health"` |  |
| healthcheck.livenessProbe.httpGet.port | string | `"http"` |  |
| healthcheck.readinessProbe.httpGet.path | string | `"/funds"` |  |
| healthcheck.readinessProbe.httpGet.port | string | `"http"` |  |
| healthcheck.readinessProbe.initialDelaySeconds | int | `10` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"647993678576.dkr.ecr.us-east-1.amazonaws.com/bestbid"` |  |
| image.tag | string | `nil` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations."cert-manager.io/cluster-issuer" | string | `"letsencrypt-cluster-issuer"` |  |
| ingress.annotations."kubernetes.io/ingress.class" | string | `"nginx"` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0].host | string | `"bestbid-api-corda.dev.pod-expand.becomeholonic.com"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls[0].hosts[0] | string | `"bestbid-api-corda.dev.pod-expand.becomeholonic.com"` |  |
| ingress.tls[0].secretName | string | `"bestbid-api-corda-dev-tls"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.port | int | `8080` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.8.1](https://github.com/norwoodj/helm-docs/releases/v1.8.1)