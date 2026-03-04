## What changed
Added docker-notes.md with Docker validation outputs.

## Why
To verify Docker installation and Postgres container setup.

## How to test
Run:
docker version
docker run hello-world
docker logs pg-prework

Expected: Postgres logs show "database system is ready to accept connections".

## Scope
Documentation only.
