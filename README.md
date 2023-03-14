# dockerpi
A repository of docker images for use on a Raspberry Pi

## Pi-Hole

Basic Docker Compose image using the pi-hole container. Remember to add a local `.env` file with the following parameters:
* `PI_HOLE_TZ=Australia/Brisbane` (just do a `cat /etc/timezone` and pop the result in here)
* `PI_HOLE_PWD=superSecr3tP@$$w0rd` which will be your admin password. Try `openssl rand -base64 12` for something a little more secure than `pass@word1`
