## Paperless-ngx
[Link to docs](https://docs.paperless-ngx.com/)

## Install Paperless-ngx
Installation Script ([src](https://docs.paperless-ngx.com/setup/))
```sh
bash -c "$(curl --location --silent --show-error https://raw.githubusercontent.com/paperless-ngx/paperless-ngx/main/install-paperless-ngx.sh)"
```

## Backups
```bash
#!/bin/bash
cd /path/to/paperless-ngx
docker compose exec -T webserver document_exporter /usr/src/paperless/export -z
```