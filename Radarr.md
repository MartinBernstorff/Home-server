##Reference

```docker run --restart=always --name=radarr -v /home/martin/docks/radarr:/config -v /home/martin/torrents:/downloads -v /home/martin/torrents/movies:/movies -v /etc/localtime:/etc/localtime:ro -e PGID=1000 -e PUID=1000 -p 7878:7878 linuxserver/radarr```