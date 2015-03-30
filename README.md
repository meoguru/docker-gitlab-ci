# Setting up GitLab CI

GitLab CI deployment with integrated PostgreSQL and Redis.

## Requirements

* [Docker](https://www.docker.com) and [Docker Compose](https://docs.docker.com/compose).
* [nginx-proxy](https://github.com/jwilder/nginx-proxy) to act as a reverse proxy.

## Installation

```sh
cp env/postgresql.env.example env/postgresql.env
cp env/ci.env.example env/ci.env

# Edit configuration files for your own need

# For nginx-proxy's virtual-host settings, kindly refer to:
# https://github.com/jwilder/nginx-proxy#usage

# For GitLab CI settings, kindly refer to:
# https://github.com/sameersbn/docker-gitlab-ci#available-configuration-parameters

docker-compose up -d
```

## Upgrade

Please refer to instruction [here](https://github.com/sameersbn/docker-gitlab-ci#upgrading).

## License

MIT licensed.
