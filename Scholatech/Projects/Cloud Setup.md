
## Stack
- Laravel + inertiaJs + Vuejs 3 + MySql
## Devops
- we need a docker composer setup we can server out app through HTTPS.
- we need to ensure that the setup is secure and try to create backups of the database daily in a a systimatic way 
### Solutions
- Im considering a docker/docker compose setup where i use Caddy or Traefik, as for the database i want a dockerised instance of mysql. 
- I want to set up the secrets for the .env file and set up a ci/cd workflow using github actions and make sure that my devops setup is secure and up to standards and good practices.