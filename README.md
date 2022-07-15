# autogit

>Tool for lazy linux developers.
Automate the Git authentication process.
Automatically inserts username and password (token).
This data is stored in /home/[user]/.autogit/supersecrets, previously encrypted for security.
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
- run ```autogit saio "commit msg example"``` for execute a "simple all in one" command aka ```git add .```, ```git commit -m "commit msg example"``` and ```git push```.
- run ```autogit add *``` like ```git add *```.
- run ```autogit uninstall --purge``` to complete uninstall this tool.

#### tips
- ```autogit --help``` or ```autorgit -h``` for help
- ```autogit --version``` or ```autorgit -v``` for version

---

# Last updates
- modified man page
- fixed some bugs
- improved encr

---

# TODO
- testing

---

#### version BETA 0.4.2

