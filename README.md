# AMS User Manual

User documentation for the Blinken OSA Archivum Archival Management System (AMS).

## Local preview

```shell
python3 -m pip install -r requirements.txt
mkdocs serve
```

Then open <http://127.0.0.1:8000>.

## Build

```shell
mkdocs build --strict
```

The documentation source is in `docs/`; navigation and theme settings are in `mkdocs.yml`.

## Production with Docker Compose

The production stack builds the MkDocs site into an immutable Nginx image and exposes it only on a configurable local port. The MkDocs development server is not used in production. Forward the public hostname from the server's existing reverse proxy to this local port.

Copy the example environment file and start the stack:

```shell
cp .env.example .env
docker compose up --build -d
```

On servers with the legacy standalone Compose command, use `docker-compose up --build -d` instead. The Compose file uses the legacy-compatible 3.3 schema.

The manual is available at <http://127.0.0.1:8080> by default. Change `AMS_MANUAL_PORT` in `.env` to use another local port. Keep `AMS_MANUAL_BIND_ADDRESS=127.0.0.1` so the container cannot bypass the host reverse proxy.

For example, the relevant location in the existing host Nginx virtual host can forward requests to the default port:

```nginx
location / {
    proxy_pass http://127.0.0.1:8080;
    proxy_set_header Host $host;
    proxy_set_header X-Real-IP $remote_addr;
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
    proxy_set_header X-Forwarded-Proto $scheme;
}
```

Check the containers and the proxy health endpoint:

```shell
docker compose ps
curl --fail http://127.0.0.1:8080/healthz
```

Rebuild after changing the documentation:

```shell
docker compose up --build -d
```

Stop the stack without removing its built image:

```shell
docker compose down
```
