# Technical Prerequisites

## Obtaining Releases

The most recent release of Tractus-X EDC can be obtained under `https://github.com/eclipse-tractusx/tractusx-edc/releases`.
To create your own build, you can clone the repository at `https://github.com/eclipse-tractusx/tractusx-edc` and consult the provided README.md.
This can be useful if you want to use non-standard extensions or configuration.

## Container Environment

Tractus-X releases come in the form of Docker containers and corresponding Helm charts.
As such, recent versions of the following are required.

- Docker
- Kubernetes
- Helm

Seeing as these are standard tools, Tractus-X EDC will run on any cloud environment that can accept Helm charts.

## Backend Dependencies

The EDC requires backend services for persistence of data and secrets. The following backends are currently supported.

Data Storage:

- PostgreSQL database
- In memory database

Secret Storage:

- Hashicorp Vault
- Azure Vault

The default setup assumes data storage via PostgreSQL database.
In memory storage is only recommended for running tests.
Hashicorp Vault is the default secret provider, because it is platform-agnostic.

Helm charts are provided to set up these services locally.
**These are not suited for production environments.**

## All-in-one deployment

An all-in-one deployment is no longer in scope and will not be provided.

## NOTICE

This work is licensed under the [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0).

- SPDX-License-Identifier: Apache-2.0
- SPDX-FileCopyrightText: 2021,2022,2023 Contributors to the Eclipse Foundation
- Source URL: <https://github.com/eclipse-tractusx/tractusx-edc>
