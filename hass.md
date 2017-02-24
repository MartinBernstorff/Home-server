# HASS
---
|  Key  | Value  |
| --- | --- |
|User| `hass` |
|Group| `hass`|
|Install dir| `/serv/hass/`|
|Config alis| `~/.homeassistant/`
|Config dir| `/home/hass/.homeassistant/`
|Log dir| `/home/hass/.homeassistant/`|
|Upstart script| `/etc/systemd/system/hass.service`|
|Port|`8123`|

## Upgrading home assistant
##### 1. Become the new user
``` bash
sudo su -s /bin/zsh hass
```

Replace `/bin/zsh` with `/bin/bash` if you're running the default shell.
##### 2. Activate the virtualenv
``` bash
source /srv/hass/bin/activate
```
##### 3. Upgrade home assistant
``` bash
pip3 install --upgrade homeassistant
```
