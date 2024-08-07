# Kickstart Example Docker Compose Configurations

Lightweight Docker compose configuration used in guides to quickly spin up FusionAuth locally with configurations from a kickstart for demonstration with no need for OpenSearch.

## Project Contents

The `docker-compose.yml` file and the `kickstart` directory are used to start and configure a local FusionAuth server. The `.env` file contains the environment variables used by the FusionAuth instance.


## Running FusionAuth

To start FusionAuth run the following command:

```
docker compose up
```

This will start a PostgreSQL and FusionAuth server.

FusionAuth will initially be configured with these settings:

* Your client id is: `e9fdb985-9173-4e01-9d73-ac2d60d1dc8e`
* Your client secret is: `super-secret-secret-that-should-be-regenerated-for-production`
* Your example username is `richard@example.com` and your password is `password`.
* Your admin username is `admin@example.com` and your password is `password`.
* Your API key is `33052c8a-c283-4e96-9d2a-eb1215c69f8f-not-for-prod`
* Your FusionAuth URL is 'http://localhost:9011/'


## Kickstart

More information around kickstart is available at https://fusionauth.io/docs/get-started/download-and-install/development/kickstart and docker compose related kickstart documentation at https://fusionauth.io/docs/get-started/download-and-install/docker#kickstart.
