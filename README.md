# Kodi installation on debian (10) without X-Server
This document provide simple way to installation kodi ui on debian without graphic environment, without installation gnome, kde, fxce.

## Steps:
### 1. Install debian os. 
* For installation debian os I recommend download debian-10.xx.xx-amd64-netinst.iso from official site. We don't need a more powerful distribution.
* U can install os use gpahichal or no-graphical ui it's never mind.
* Create default user with name "user"
* All installation parameters can be default, but in "Software selection" menu u need disable "Debian desktop environment". We want to install os without any graphical components. 
<img src="https://raw.githubusercontent.com/ReyStar/kodi_installation/master/man/dea638a4-2fa0-4b30-b661-e37c864beb03.png" alt="dea638a4-2fa0-4b30-b661-e37c864beb03.png" width="500"/>

### 2. Install lightdm
LightDM is a cross-desktop display manager. It was built as a relatively light-weight and highly customizable alternative to GDM.
https://wiki.debian.org/LightDM
* for installatin use commnd `apt install lightdm`
* For autologin user set in config file `/etc/lightdm/lightdm.conf` next value autologin-user=user
* For autostart kodi application after user login set in config file `/etc/lightdm/lightdm.conf` next value display-setup-script=kodi

[config example](https://github.com/ReyStar/kodi_installation/blob/master/man/lightdm.conf)

### 3. Install kodi
* For kodi installation use command `apt-get install kodi`

### 4. Result
* Reboot and enjoy
<img src="https://raw.githubusercontent.com/ReyStar/kodi_installation/master/man/e1a2f19c-0d22-4834-ac6d-324c6464d3b1.png" alt="e1a2f19c-0d22-4834-ac6d-324c6464d3b1.png" width="500"/>
