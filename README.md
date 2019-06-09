# RAMmy Pihole in Docker
This is my Pihole container using ramdisks to minimize wear and tear on my RPi SD cards. I think.
That may be urban legend. It's a fun project.

Based on: https://github.com/pi-hole/docker-pi-hole

## Instructions

1. Edit the `docker_compose.yml` file:
  a. Change service `ipv4_address` and network `subnet` properties as appropriate
  b. Change the service `dns` properties if desired
2. Set the Pihole admin password you want to use in the DOCKER_PIHOLE_ADMIN_PW environment variable
3. `docker-compose up`
4. Confirm Pihole is running by broswing to the address set in `ipv4_address`
