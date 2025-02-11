open terminal: <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>t</kbd>
## files and directories
create new file
```shell
touch FILE-NAME
```
create new directory
```shell
mkdir DIRECTORY-NAME
```
## apt
update apt package list (to obtain information on newest versions)
```shell
apt update
```
fetch newest versions of apt packages and remove packages if necessary
```shell
apt full-upgrade
```
remove obsolete packages after upgrade or removal
```shell
apt autoremove
```
install apt packages on the system
```shell
apt install PACKAGE-NAME
```
remove apt packages from the system
```shell
apt remove PACKAGE-NAME
```
## snap
update snap packages
```shell
snap refresh
```
install snap packages on the system
```shell
snap install PACKAGE-NAME
```
remove snap packages from the system
```shell
snap remove PACKAGE-NAME
```
## ClamAV
update signature databases
```shell
freshclam
```
scan all files in current directory
```shell
clamscan --recursive .
```
scan all files on system
```shell
clamscan --recursive /
```
## VS Code
open in current directory
```shell
code .
```
open VS Code terminal: <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>`</kbd>
## Python venv
create venv
```shell
python -m venv venv
```
activate venv
```shell
source venv/bin/activate
```
deactivate venv
```shell
deactivate
```
install required packages
```shell
pip install -r requirements.txt
```
## ImageMagick
convert image file format (v6.9.12)
```shell
convert FILE-NAME FILE-NAME
```