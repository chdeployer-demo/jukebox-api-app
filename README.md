# Jukebox API App

An example MuleSoft application used to demonstrate [Anypoint CloudHub Deployment CLI](https://github.com/Redpill-Linpro/anypointchdeployer).

## Overview

This is a Mule 4 application that implements a simple Jukebox API. It serves as a reference project for testing and demoing automated deployments to Anypoint CloudHub using the Anypoint CloudHub Deployment CLI tool.

## Deployment Approach

This project uses only the standard [Mule Maven Plugin](https://docs.mulesoft.com/mule-runtime/latest/mmp-concept) to deploy artifacts to Anypoint Exchange. No additional deployment plugins or custom tooling is required — the actual CloudHub deployment is handled separately by the [Anypoint CloudHub Deployment CLI](https://github.com/Redpill-Linpro/anypointchdeployer).

## Prerequisites

- Java 17
- Maven 3.x
- MuleSoft Anypoint Platform account

## Building

```bash
mvn clean package
```

## Deploying

```bash
mvn deploy
```

A GitHub Actions workflow is included for manual build and deploy. See [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml).

## License

This project is licensed under the Apache License 2.0 — see [LICENSE.md](LICENSE.md) for details.
