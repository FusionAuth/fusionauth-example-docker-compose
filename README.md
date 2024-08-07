# Example Docker Compose Configurations

This repository contains different FusionAuth docker compose configuration examples used in the [Using FusionAuth on Docker](https://fusionauth.io/docs/get-started/download-and-install/docker) documentation.

## Contents

There are multiple examples, one directory for each.

### build

An example which builds Example Password Hasher Plugin and adds it in to a custom fusionauth-app image.

### kickstart

A complex example using kickstart to stage a development FusionAuth environment.

### light

A lightweight Docker compose configuration used in guides to quickly spin up FusionAuth locally with configurations from a kickstart for demonstration with no need for OpenSearch.

### mailcatcher

An example which stages a development FusionAuth environment including mailcatcher which allows FusionAuth to send transactional emails for account verification, password reset, and others in your development environment.

### plugin

An example which builds an Example Password Hasher Plugin with a maven init-container and adds it in to a mounted directory. Which then, when built successfully, gets directly mounted as a directory in to your FusionAuth Docker container.

## Dependencies
* Docker, for running FusionAuth and related services.

## Running FusionAuth examples
To run FusionAuth, just change in to one of the example directories and stand up the docker containers using `docker compose`.

```shell
docker compose up -d
```

This will start the FusionAuth example with the related services.

To fully remove the example you have to remove the volumes too by running the following command inside the according example directory

```shell
docker compose down -v
```
