# Test simple dummy apis with Kubernetes

This repository contains a collection of Kubernetes templates designed for testing and development purposes. These templates provide a standardized way to deploy, manage, and scale containerized applications in a Kubernetes cluster.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Templates Overview](#templates-overview)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Kubernetes is a powerful orchestration tool for managing containerized applications. This repository aims for just a training process of testing Kubernetes deployments by providing a set of ready-to-use templates. These templates can be used to quickly set up various components and services, ensuring a consistent and reliable environment for development and testing.

## Getting Started

To get started, clone this repository and navigate to the directory containing the templates. Make sure you have a Kubernetes cluster up and running, and that you have `kubectl` configured to interact with your cluster.

```sh
git clone https://github.com/svestor/kube-net.git
cd kube-net
```

## Templates Overview

The repository includes templates for various Kubernetes resources, such as:

- Deployments
- Services
- ConfigMaps
- Secrets
- Persistent Volume Claims
- Ingress

Each template is designed to be easily customizable and reusable. The following sections provide examples and usage instructions for each type of resource.

## Usage

To use a template, simply apply it to your Kubernetes cluster using `kubectl`. For example, to deploy a sample application, navigate to the appropriate directory and run:

```sh
kubectl apply -f deployment.yaml
```

You can modify the template files to suit your needs before applying them. Refer to the Kubernetes documentation for detailed information on each resource type.

## Customization

Each template is designed to be flexible and easy to customize. You can change parameters such as image versions, resource limits, and environment variables by editing the YAML files. For example, to change the image used in a deployment, update the `image` field in `deployment.yaml`:

```yaml
spec:
  containers:
    - name: my-app
      image: my-app:latest
```

Feel free to adapt the templates to match your specific requirements.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
