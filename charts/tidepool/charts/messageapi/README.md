# messageapi

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![AppVersion: 1.0](https://img.shields.io/badge/AppVersion-1.0-informational?style=flat-square)

A Helm chart for Kubernetes

**Homepage:** <https://github.com/tidepool-org/development/charts>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| deployment.env.window | int | `21` |  |
| deployment.image | string | `"tidepool/message-api:master-latest"` | Docker image |
| deployment.replicas | int | `1` |  |
| hpa.enabled | bool | `false` | whether to create a horizontal pod autoscalers for all pods of given deployment |
| hpa.maxReplicas | string | `nil` | maximum number of replicas that HPA will maintain |
| hpa.minReplicas | int | `1` | minimum number of replicas that HPA will maintain |
| mongo.secretName | string | `"mongo"` |  |
| nodeEnvironment | string | `"production"` |  |
| nodeSelector | object | `{}` |  |
| pdb.enabled | bool | `false` |  |
| pdb.minAvailable | string | `"50%"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| tolerations | list | `[]` |  |