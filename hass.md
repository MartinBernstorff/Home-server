# HASS
---

Home assistant is installed in a virtualenv under user ```hass``` in the directory ```/serv/hass```

## Upgrading home assistant
##### 1. Become the new user
```
sudo su -s /bin/zsh hass
```

Replace `/bin/zsh` with `/bin/bash` if you're running the default shell.
##### 2. Activate the virtualenv
```
source /srv/hass/bin/activate
```
##### 3. Upgrade home assistant
```
pip3 install --upgrade homeassistant
```
