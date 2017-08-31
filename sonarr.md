```
docker run \
	--restart=always
    --name sonarr \
    -p 8989:8989 \
    -e PUID=1000 -e PGID=1000 \
    -v /etc/localtime:/etc/localtime:ro \
    -v /home/martin/docks/sonarr/config:/config \
    -v /home/martin/torrents/tv:/tv \
    -v /home/martin/torrents/tv:/downloads \
    linuxserver/sonarr
```