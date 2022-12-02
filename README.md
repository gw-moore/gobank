# Go Bank

Toy project for me to learn to go. Go Bank is a REST API for a banking service.

## Setup

Use docker to setup a postgres database to interactive with during development.

```bash
docker run --name gobank-postgres -e POSTGRES_PASSWORD=gobank -p 5432:5432 -d postgres
```

Once the docker container is running, use the `make run` command to start the API server

## Example API requests

- Create account -> POST request to `localhost:3000/account/`
- Get all accounts -> GET request to `localhost:3000/account`
- Get specific account -> GET request to `localhost:3000/account/{id}`
