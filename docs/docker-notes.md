# Docker Validation Notes

## Docker Version
Command:
docker version

This confirms Docker is installed correctly.

## Hello World Test

Command:
docker run hello-world

Result:
Docker successfully ran the hello-world container.

## Postgres Container

Command:
docker run --name pg-prework -e POSTGRES_PASSWORD=postgres -d postgres

This starts a postgres container.

## Check Logs

Command:
docker logs pg-prework

Log output includes:

database system is ready to accept connections

## Stop Container

Command:
docker stop pg-prework

## Restart Container

Command:
docker restart pg-prework
