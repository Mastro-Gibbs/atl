# atl

>Tool for lazy linux developers.
Automate the Git authentication process.
Automatically inserts username and password (token).
This data is stored in /home/[user]/.atl/supersecrets, previously encrypted for security.
---

## Supported packages manager 
- [x] apt / apt-get
- [x] dnf
- [x] pacman
- [x] yum
- [x] xbps

---

## Guide

#### installing
- run ```./installer --configure``` to run installer script. ```--configure``` option will run the configuration script entirely.
By default the executable will be copyied into /usr/local/bin.
- run ```./installer --configure --prefix <path>``` to run installer script. ```--configure``` option will run the configuration script entirely. ```--prefix <path>``` option will specify the location into install it.

### usages
- run ```atl saio "commit msg example"``` for execute a "simple all in one" command aka ```git add .```, ```git commit -m "commit msg example"``` and ```git push```.
- run ```atl add *``` like ```git add *```.
- run ```atl uninstall --purge``` to complete uninstall this tool.

#### tips
- ```atl --help``` or ```autorgit -h``` for help
- ```atl --version``` or ```autorgit -v``` for version

---

# Last updates
- modified man page
- fixed some bugs
- improved encr

---

# TODO
- testing

---

#### version BETA 0.1.2

