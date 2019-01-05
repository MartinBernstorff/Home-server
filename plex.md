```
docker run -d \
--restart=always \
--name=plex \
--net=host \
-e VERSION=latest \
-e PUID=1000 -e PGID=1000 \
-e TZ=Europe/Copenhagen \
-v /home/martin/docks/plex/config:/config \
-v /home/martin/torrents/tv:/data/tvshows \
-v /home/martin/torrents/movies:/data/movies \
-v /home/martin/docks/plex/transcode:/transcode \
linuxserver/plex
```

To upgrade:

```bash
docker stop plex
docker rm -f plex
docker pull linuxserver/plex
```

Then run the above command