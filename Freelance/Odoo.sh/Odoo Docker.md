I want to deploy an odoo instance on coolify based on a docker and docker compose files setup 
how do i build this image and push it to the dockerhub and fetch it in my coolify service ? Build this and push it locally and fetch it from coolify that is deployed in a server

- i have the following docker-compose file:
```yaml
services:
  odoo:
    image: 'odoo:17'
    environment:
      - SERVICE_FQDN_ODOO_8069
      - HOST=postgresql
      - USER=$SERVICE_USER_POSTGRES
      - PASSWORD=$SERVICE_PASSWORD_POSTGRES
    volumes:
      - 'odoo-web-data:/var/lib/odoo'
    healthcheck:
      test:
        - CMD
        - curl
        - '-f'
        - 'http://127.0.0.1:8069'
      interval: 2s
      timeout: 10s
      retries: 30
  postgresql:
    image: 'postgres:16-alpine'
    volumes:
      - 'postgresql-data:/var/lib/postgresql/data'
    environment:
      - POSTGRES_USER=$SERVICE_USER_POSTGRES
      - POSTGRES_PASSWORD=$SERVICE_PASSWORD_POSTGRES
      - POSTGRES_DB=postgres
    healthcheck:
      test:
        - CMD-SHELL
        - 'pg_isready -U $${POSTGRES_USER} -d postgres'
      interval: 5s
      timeout: 20s
      retries: 10
```
I want to build a custom Odoo docker image that uses the odoo:17 and modify my docker-compose file to use
*TODO: 
	- Help me build the custom the custom docker image locally and test it using the docker-compose
		- if the build and testing is succesful i want to use the setup on coolify*

```
dujf-wjyg-dyge
```

docker compose exec postgresql psql -U odoo -d alkhayat-db-2

SELECT id, login 
FROM res_users 
WHERE login = 'hargousse.hicham@gmail.com';

	UPDATE res_users 
	SET password = 'admin'
	WHERE login = 'hargousse.hicham@gmail.com';

UPDATE res_users 
SET password = 'admin'
WHERE login = 'hargousse.hicham@gmail.com';


The style compilation failed. This is an administrator or developer error that must be fixed for the entire database before continuing working. See browser console or server logs for details.



