# prometheus-statsd-exporter

Prometheus Exporter for [Statsd](https://github.com/statsd/statsd) metrics.

This chart bootstraps a [Statsd Exporter](https://github.com/prometheus/statsd_exporter) deployment on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

## Prerequisites

- Kubernetes 1.16+ with Beta APIs enabled
- Helm 3+

## Get Repo Info

```console
helm repo add nholuongut https://github.com/nholuongut/helm-charts
helm repo update
```

_See [helm repo](https://helm.sh/docs/helm/helm_repo/) for command documentation._

## Install Chart

```console
helm install [RELEASE_NAME] nholuongut/prometheus-statsd-exporter
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

```console
helm upgrade [RELEASE_NAME] [CHART] --install
```

_See [helm upgrade](https://helm.sh/docs/helm/helm_upgrade/) for command documentation._

## Configuring

See [Customizing the Chart Before Installing](https://helm.sh/docs/intro/using_helm/#customizing-the-chart-before-installing). To see all configurable options with detailed comments, visit the chart's [values.yaml](./values.yaml), or run these configuration commands:

```console
helm show values nholuongut/prometheus-statsd-exporter
```

### Statsd Exporter Server

- Use early created ConfigMap with file `statsd.mappingConf` contained in data or specify mapping values in `statsd.mappingConfig`
