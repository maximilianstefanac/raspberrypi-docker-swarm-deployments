# Nextcloud Stack

## How to deploy
1. create a file called `secrets.env` in the folder where the `docker-compose-rpi-nextcloud.yml` file is placed.
2. Add contents for following environment variables:
    * `POSTGRES_DB`,
    * `POSTGRES_USER`,
    * `NEXTCLOUD_ADMIN_USER`,
    * `NEXTCLOUD_ADMIN_PASSWORD` and
    * `NEXTCLOUD_TRUSTED_DOMAINS`.
3. Execute: `docker stack deploy --compose-file=docker-compose-rpi-nextcloud.yml nextcloud`. Aditionally, you could name the stack other than `nextcloud`.