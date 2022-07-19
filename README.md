# ATL

ATL is a tool available on GNU/Linux systems that allows you to automate various login and authentication mechanisms such as those required by git and ssh.

---

## Supported package managers 
- [x] apt / apt-get
- [x] dnf
- [x] pacman
- [x] yum
- [x] xbps

---

## Installation

Clone or fork this repository, get the source code, run:



```bash
$ ./install --configure --prefix=<preferred_installation_path>
```
The interactive installer will start, it will ask you if you want to generate a soft link in ```/usr/local/bin``` for the executable and three soft links for the manual pages in ```/usr/share/man/man1```.  
It's up to you to choose whether to create them or not.  
In case of reinstallation, the script will identify the previous installation and will ask whether to overwrite it or not.  
In both cases the previous installation will be removed.
##### Explanation:
* ```--configure``` will run the configuration script which will check the dependencies needed for the main script to work.
* ```--prefix=<some_path>``` set the preferred installation path, preferably it should start from ```/home/<user>/```, otherwise errors could be generated.

---

## Uninstall
##### There are two ways to go:
* Tool only removal
```bash
$ atl uninstall
```

* Tool and configuration folder removal
```bash
$ atl uninstall --purge
```
---

## GIT and SSH configure
* For **git** run the following command.  
A script will be executed that will interactively ask for credentials, which will be **encrypted** and saved in ```/home/<user>/.atl/git/```.
```bash
$ atl config git
```   

* For **ssh** run the following command.  
A script will be executed that will interactively ask for the credentials, which will be **encrypted** and saved in a **relative** and **personal folder** for the host entered, in ```/home/<user>/.atl/ssh/```.
```bash
$ atl ssh add
```
or, but read man page for atl
```bash
$ atl config ssh
```


---

## Usage

```bash
$ atl git push origin <branch_name>
```
```bash
$ atl git saio <commit_message>
```
```bash
$ atl ssh connect
```
#### See man page for more:
- **atl**(1)
- **atl-git**(1)
- **atl-ssh**(1)

---

## Version
BETA 0.3

## License
[GPLV3](https://github.com/Mastro-Gibbs/atl/blob/main/LICENSE.md)