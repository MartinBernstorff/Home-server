# HASS
---


```bash
docker run -d --restart=always --name="home-assistant" -v /home/martin/docks/HASS:/config -v /etc/localtime:/etc/localtime:ro --net=host homeassistant/home-assistant
```

Upgrading:

```bash
docker stop home-assistant
docker rm -f home-assistant
docker pull homeassistant/home-assistant
```

Then run the above