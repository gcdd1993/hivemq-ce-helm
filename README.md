# Helm Chart for hivemq-ce

> Just for test

# TL;DR

```bash
# Testing configuration
$ helm repo add hivemq-ce-helm https://github.com/gcdd1993/hivemq-ce-helm
$ helm install my-hivemq gcdd1993/hivemq-ce-helm
```

# Parameters

| **Parameter**    | **Description**                                              | **Default**      |
| ---------------- | ------------------------------------------------------------ | ---------------- |
| replicaCount     | pod replica count                                            | 1                |
| image.registry   | Hivemq-ce Image registry                                     | docker.io        |
| image.repository | Hivemq-ce Image name                                         | hivemq/hivemq-ce |
| image.tag        | Hivemq-ce Image tag                                          | latest           |
| image.pullPolicy | Image pull policy                                            | IfNotPresent     |
| imagePullSecrets | Specify docker-registry secret names as an array             | nil              |
| nameOverride     | String to partially override redis.fullname template with a string (will prepend the release name) | nil              |
| fullnameOverride | String to fully override redis.fullname template with a string | nil              |
| service.type     | Kubernetes Service type                                      | NodePort         |
| service.port     | Kubernetes Service port                                      | 1883             |
| service.nodePort | Kubernetes Service nodePort                                  |                  |
|                  |                                                              |                  |

