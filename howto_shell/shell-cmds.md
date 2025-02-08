## apt
update apt package list (to obtain information on newest versions)
```bash
apt update
```
fetch newest versions of apt packages and remove packages if necessary
```bash
apt full-upgrade
```
remove obsolete packages after upgrade or removal
```bash
apt autoremove
```
install apt packages on the system
```bash
apt install [package-name]
```
remove apt packages from the system
```bash
apt remove [package-name]
```
## snap
update snap packages
```bash
snap refresh
```
install snap packages on the system
```bash
snap install [package-name]
```
remove snap packages from the system
```bash
snap remove [package-name]
```
## ClamAV
update signature databases
```bash
freshclam
```
scan all files in current directory
```bash
clamscan --recursive .
```
scan all files on system
```bash
clamscan --recursive /
```