# docker-compose-duplicati-haproxy-conf
Deploy duplicati with haproxy as proxy in a doker container using docker-compose.

Clone project, copy default.env to.env and edit.

Start with "docker-compose up -d".

To block the access to duplicati while it's still running, use "docker-compose stop haproxy".

Restart haproxy with "docker-compose start haproxy".

Stop and remove with "docker-compose down".

I have bwdata and duplicati folders added in docker-compose.yml so duplicati can see them for backup, bwdata is used by Bitwarden.
