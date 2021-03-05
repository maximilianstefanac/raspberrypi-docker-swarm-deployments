# Pi-hole Stack

## How to deploy
1. create a file called `config.env` in the folder where the `docker-compose-rpi-pihole.yml` file is placed.
2. Add contents for following environment variables. See [here](https://hub.docker.com/r/pihole/pihole) for description of these variables.
    * `TZ` and
    * `ServerIP`
3. create a file called `secrets.env` in the folder where the `docker-compose-rpi-pihole.yml` file is placed.
4. Add content for following environment variable. See [here](https://hub.docker.com/r/pihole/pihole) for description of this variable.
    * `WEBPASSWORD`
1. Execute: `docker stack deploy --compose-file=docker-compose-rpi-nextcloud.yml nextcloud`. Aditionally, you could name the stack other than `nextcloud`.