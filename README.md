# Schier Kubernetes OpenTelemetry Helm Chart

This repository contains the Helm chart and the associated values to install the OpenTelmetry Collector into a Kubernetes cluster with the associated ingestion tokens for Mezmo 

## TL;DR;

```console
$ helm repo add mezmo-otel-collector https://github.com/schierproducts/kubernetes-opentelemetry-collector
$ helm upgrade -i --create-namespace -n mezmo \
    mezmo-otel-collector schierproducts/kubernetes-opentelemetry-collector
```

### To use Locally

To use this locally without adding this repository as a helm repository, clone the repository and within the new directory run the following command:

```console
helm upgrade -i --create-namespace -n mezmo \
  mezmo-otel-collector .
```

## To Uninstall

To uninstall this Helm chart from the cluster, run the following command:

```console
helm uninstall -n mezmo mezmo-otel-collector
```