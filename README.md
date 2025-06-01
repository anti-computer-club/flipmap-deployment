# What's This?

Code and actions that deploy the [flipmap-backend](https://github.com/anti-computer-club/flipmap-backend) and other associated services into production. This is an infrastructure repository that supports the greater FlipMap project. [**FlipMap is the Map App for Flip-phones!**](https://anticomputer.club/)

`.env-example` provides a minimum-viable example of what environment variables are needed to deploy the backend and reverse proxy given the example Caddyfile.

`/Caddy/` provides the Dockerfile and the Caddyfile which is copied into the container at build time.

`compose.yaml` is the project's singular compose.

Other repositories build, push, and pull their individual containers. This repository just builds and pushes supporting services. It will pull all containers and restart the compose entirely when updated.

## License

This repository is licensed under the GNU General Public License Version 2 and any later version.

## Roadmap & Contribution Guidelines

This repository is provided partially as an example of deployment. Pull requests and issues are requested only for glaring errors and omissions, please do not attempt to PR features or other significant changes into this repository.

For outstanding issues across the project, see the [roadmap Github Project](https://github.com/orgs/anti-computer-club/projects/5)
