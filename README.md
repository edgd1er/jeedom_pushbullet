# jeedom_pushbullet
Pushbullet plugin for Jeedom

* travail en cours: 
  * testé uniquement sur rpi4.

# Installation
* manuel via un pull de git ou unzip 

# Differences
* Adaptations pour Jeedom 4.
* Adaptation pour python 3.
* utilisation de packages.json

# Author
Basé sur le travail de Stéphane Cazeaux

```bash
BKS="--break-system-packages"
[[ 0 -ne $(pip3 list | grep -c pushbullet-python) ]] && pip3 uninstall -y ${BKS} pushbullet-python || true
pip3 install ${BKS} websocket-client pushbullet.py pip legacy-cgi

rm /tmp/jeedom/pushbullet/pushbullet.o.Yn0TJi6KXhe9tTReiWT3iOM98e0hAofo.pid && python3 /var/www/html/plugins/pushbullet/ressources/pushbullet_daemon/pushbulletd.*

```
