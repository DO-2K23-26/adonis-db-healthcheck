# Probes POC

With `docker` only:
`docker network create -d bridge app-network`
`docker build -t monapp:0.0.1 -f Dockerfile .`
`docker run -d --network=app-network -p 3333:3333 --name=app --env-file=.env monapp:0.0.3`
`docker run -d --network=app-network -p 5432:5432 --name=app-postgres -e POSTGRES_PASSWORD=6R879G028HDIP -e POSTGRES_USER=root -e POSTGRES_DB=app postgres:17.2`

With `docker compose`:

`docker compose up -d`

Interesting commands (with `pnpm`):

`pnpm audit fix [--force]`
`pnpm outdated`
