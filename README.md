# nsea

A simple docker compose script that spins up local [Narwhal server](https://github.com/itworks99/narwhal) environment.

Tested with Debian/Ubuntu.

## How to use

### Get Docker and docker-compose

1. [Get Docker](https://docs.docker.com/install/)

2. [Install or update docker compose](https://docs.docker.com/compose/install/)

### Clone this git repository

    git clone https://github.com/itworks99/nsea.git; cd nsea

### Start with

    docker-compose up

or

    docker-compose -f "docker-compose.yml" up -d --build

### Access web dashboard

Navigate to https://127.0.0.1:3000 then create a security exception because at this point in time Narwhal is using [local security certificates](https://letsencrypt.org/docs/certificates-for-localhost/).

### Access JSON endpoints

Navigate to https://127.0.0.1:3000/json_all for all data. Use https://127.0.0.1:3000/json_alerts for alerts only.


### Download data as CSV files