# SpiceDB(An open source, Zanzibar-inspired database for permissions) 

This Docker Compose setup runs [SpiceDB Permission Database](https://github.com/authzed/spicedb) along with Postgres using `docker-compose`.

## Pre-requisites

- [Docker](https://docs.docker.com/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Authzed SpiceDB](https://github.com/authzed/spicedb)
- [Authzed SpiceDB with datastore](https://docs.authzed.com/spicedb/selecting-a-datastore)

## Usage

- Clone this repo on a machine where you'd like to deploy graphql engine
- `docker-compose up -d`

Visit http://localhost:8080 to see next steps, including loading the schema
