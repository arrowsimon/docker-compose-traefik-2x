# docker-compose-traefik-2x


```
    networks:
      - web
      - default

    labels:
      - "traefik.enable=true"
      - "traefik.http.routers.jira.rule=Host(`jira.arrowdemo.se`)"
      - "traefik.http.routers.jira.tls=true"
      - "traefik.http.routers.jira.tls.certresolver=le"
      - "traefik.http.services.jira.loadbalancer.passhostheader=true"


touch acme.json 
chmod 600 acme.json

```
