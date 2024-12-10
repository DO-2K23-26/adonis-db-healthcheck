`docker build -t monapp:0.0.1 -f Dockerfile .`
`docker run -d --env-file=.env monapp`
`docker run -d --name=app-postgres -e POSTGRES_PASSWORD=6R879G028HDIP postgres:17.2`
`docker run -d --name=app-postgres -p 5432:5432 -e POSTGRES_PASSWORD=6R879G028HDIP -e POSTGRES_USER=root -e POSTGRES_DB=app postgres:17.2`
pnpm audit fix[(--force]
pnpm outdated
