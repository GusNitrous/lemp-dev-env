## Minimal LEMP stack based on Docker

## Get Started

All command examples are described for UNIX-like systems (Linux, Mac OS).

### Prerequisites

- Make sure that you have Docker and Docker Compose installed
  - Windows or macOS:
    [Install Docker Desktop](https://www.docker.com/get-started)
  - Linux: [Install Docker](https://www.docker.com/get-started) and then
    [Docker Compose](https://github.com/docker/compose)
- Download some or all of the samples from this repository.

### Running

Before starting, you must create a `.env` file based on the `.env-template`:

```console
cp -b .env-template > .env
```

Default LEMP app stack can be run in a local environment by going into the root directory and executing:

```console
docker-compose up -d
```

Going into the app container:

```console
docker exec -it {app_container_name} bash
```

To stop and remove all containers of app run:

```console
docker-compose down
```
