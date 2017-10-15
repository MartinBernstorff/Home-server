##Docker
```
docker run -d \
    --cap-add=NET_ADMIN \
    -p 8112:8112 \
    -p 8118:8118 \
    -p 58846:58846 \
    -p 58946:58946 \
    --name=delugevpn \
    -v /home/martin/torrents:/data \
    -v /home/martin/docks/deluge/config:/config \
    -v /etc/localtime:/etc/localtime:ro \
    -e VPN_ENABLED=yes \
    -e VPN_REMOTE=179.43.156.34 \
    -e VPN_USER=p1920734 \
    -e VPN_PASS=PWu5VbdFyG \
    -e VPN_PROV=pia \
    -e STRICT_PORT_FORWARD=yes \
    -e ENABLE_PRIVOXY=no \
    -e LAN_NETWORK=192.168.1.0/24 \
    -e NAME_SERVERS=8.8.8.8,8.8.4.4 \
    -e DEBUG=false \
    -e UMASK=000 \
    -e PUID=1000 \
    -e PGID=1000 \
    binhex/arch-delugevpn
```

`https://hub.docker.com/r/binhex/arch-delugevpn/`

#Slow speeds

Had to make some hacky changes to the img and delete all other mirrors than Netherlands.

`docker exec -i -t delugevpn bash`

`cd /config/openvpn`

Remove all other mirrors.