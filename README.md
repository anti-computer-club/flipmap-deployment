# What's This?

Code and actions that deploy the [flipmap-backend](https://github.com/anti-computer-club/flipmap-backend) and other associated services into production.

`.env-example` provides a minimum-viable example of what environment variables are needed to deploy the backend and reverse proxy given the example Caddyfile.

`/Caddy/` provides the Dockerfile and the Caddyfile which is copied into the container at build time.

`compose.yaml` is the project's singular compose.

Other repositories build, push, and pull their individual containers. This repository just builds and pushes supporting services. It will pull all containers and restart the compose entirely when updated.
