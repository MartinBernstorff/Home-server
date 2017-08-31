# HASS
---
```
docker run -d --restart=always --name="home-assistant" -v /home/martin/docks/HASS:/config -v /etc/localtime:/etc/localtime:ro --net=host homeassistant/home-assistant
```