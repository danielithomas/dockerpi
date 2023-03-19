# dockerpi
A repository of docker images for use on a Raspberry Pi

## Pi-Hole

Basic Docker Compose image using the pi-hole container. Remember to add a local `.env` file with the following parameters:
* `PI_HOLE_TZ=Australia/Brisbane` (just do a `cat /etc/timezone` and pop the result in here)
* `PI_HOLE_PWD=superSecr3tP@$$w0rd` which will be your admin password. Try `openssl rand -base64 12` for something a little more secure than `pass@word1`
* `HOST_SERVER_IP=192.168.0.1` which tellsthe container about its hosts IP. This allows pi hole to be accessible via http://pi.hole/admin
