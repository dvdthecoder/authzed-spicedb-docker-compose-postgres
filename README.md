## SpiceDB(An open source, Zanzibar-inspired database for permissions) 
This Docker Compose setup runs [SpiceDB Permission Database](https://github.com/authzed/spicedb) along with Postgres using `docker-compose`.

### Pre-requisites
- [Docker](https://docs.docker.com/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Authzed SpiceDB](https://github.com/authzed/spicedb)
- [Authzed SpiceDB with datastore](https://docs.authzed.com/spicedb/selecting-a-datastore)

### Usage
- Clone this repo on a machine where you'd like to deploy SpiceDB database
- Run `docker-compose up -d`

Visit http://localhost:8080 to see next steps, including loading the schema

### Rest Interface
- SpiceDB primarily exposes its API via gRPC alternatively HTTP/JSON API are available as provided here (https://docs.authzed.com/reference/api)
- SpiceDB provides for multiple ways to connect (https://docs.authzed.com/reference/clients) 
- This image enables REST end-points 

### Rest Usage
- `curl -X POST -H "Authorization: Bearer thetokengoeshere" localhost:8443/v1/permissions/check`
