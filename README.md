# A Helm Chart for DRY job deployments

[![CircleCI](https://circleci.com/gh/cetic/helm-job.svg?style=svg)](https://circleci.com/gh/cetic/helm-job/tree/master) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![version](https://img.shields.io/github/tag/cetic/helm-job.svg?label=release)

## Introduction

This helm chart define a common structure to deploy kubernetes jobs.

The goal is to provide a DRY job deployment mechanism with some flexibility, to be used with some other charts orchestrating a series of jobs via dependencies, pointing to this chart, where each instance of this chart is differenciated using aliases.

The federating chart will provide the configuration for each jobs in its values file.

## Prerequisites

- Kubernetes cluster 1.10+
- Helm 3.0.0+
- PV provisioner support in the underlying infrastructure.

## Installation

### Add Helm repository

```bash
helm repo add cetic https://cetic.github.io/helm-charts
helm repo update
```

### Configure the chart

The following items can be set via `--set` flag during installation or configured by editing the `values.yaml` directly (need to download the chart first).

TBD

### Install the chart

Install the job helm chart with a release name `my-release`:

```bash
helm install my-release cetic/job
```

## Uninstallation

To uninstall/delete the `my-release` deployment:

```bash
helm uninstall my-release
```

## Configuration

The following table lists the configurable parameters of the job chart and the default values.

| Parameter                                                                   | Description                                                                                                        | Default                         |
| --------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------| ------------------------------- |

TBD

## Contributing

Feel free to contribute by making a [pull request](https://github.com/cetic/helm-job/pull/new/master).

Please read the official [Contribution Guide](https://github.com/helm/charts/blob/master/CONTRIBUTING.md) from Helm for more information on how you can contribute to this Chart.

## License

[Apache License 2.0](/LICENSE)
