# TMC GitOps EPC

This project demonstrates the capabilities of Tanzu Mission Control (TMC) in a customer demo focused on continuous delivery.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Kustomize Configuration](#kustomize-configuration)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository serves as a practical demonstration of implementing GitOps practices using Tanzu Mission Control to manage Kubernetes clusters effectively.

## Prerequisites

- Access to a Kubernetes cluster
- Tanzu Mission Control
- Git installed

## Installation

```bash
git clone https://github.com/skandpurohit/tmc-gitops-epc.git
cd tmc-gitops-epc
```

## Usage

Deploy the application using Kustomize:

```bash
kubectl apply -k base/
kubectl apply -k overlay/
```

## Kustomize Configuration

This project uses Kustomize to manage Kubernetes configurations with a base and overlay structure. The base directory contains generic resource definitions, while overlays allow for environment-specific modifications.

### Base

Core Kubernetes resource configurations that are used as a foundation.

### Overlay

Customizations applied to the base depending on the deployment environment (development, staging, production).

## Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request with your changes.

## License

Distributed under the MIT License. See `LICENSE` for more information.
