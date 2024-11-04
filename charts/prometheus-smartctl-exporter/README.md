# Prometheus smartctl Exporter

Prometheus smartctl Exporter makes _smartctl_ statistics available to Prometheus for scraping.

For more information on the exporter, please see the project's [repository](https://github.com/nholuongut/smartctl_exporter).

## Prerequisites

- Kubernetes 1.13+ with Beta APIs enabled
- Helm 3
- smartmontools 7.0+

## Get Repository Info
<!-- textlint-disable terminology -->
```console
helm repo add nholuongut https://github.com/nholuongut/helm-charts
helm repo update
```

_See [helm repo](https://helm.sh/docs/helm/helm_repo/) for command documentation._
<!-- textlint-enable -->
## Install Chart

```console
helm install [RELEASE_NAME] nholuongut/prometheus-smartctl-exporter
```

_See [configuration](#configuration) below._

_See [helm install](https://helm.sh/docs/helm/helm_install/) for command documentation._

## Uninstall Chart

```console
helm uninstall [RELEASE_NAME]
```

This removes all the Kubernetes components associated with the chart and deletes the release.

_See [helm uninstall](https://helm.sh/docs/helm/helm_uninstall/) for command documentation._

## Upgrading Chart

```shell
helm upgrade [RELEASE_NAME] nholuongut/prometheus-smartctl-exporter --install
```

_See [helm upgrade](https://helm.sh/docs/helm/helm_upgrade/) for command documentation._

## Configuration

See [Customizing the Chart Before Installing](https://helm.sh/docs/intro/using_helm/#customizing-the-chart-before-installing). To see all configurable options with detailed comments, visit the chart's [values.yaml](./values.yaml), or run these configuration commands:

```console
helm show values nholuongut/prometheus-smartctl-exporter
```
