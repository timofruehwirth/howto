open terminal: <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>t</kbd>
## files and directories
navigate to child directory
```shell
cd DIRECTORY-NAME
```
navigate to parent directory
```shell
cd ..
```
navigate to sibling directory
```shell
cd ../DIRECTORY-NAME
```
navigate to user directory
```shell
cd ~
```
create new file
```shell
touch FILE-NAME
```
copy (and rename) file
```shell
cp FILE-NAME FILE-NAME
```
delete file
```shell
rm FILE-NAME
```
create new directory
```shell
mkdir DIRECTORY-NAME
```
remove non-empty directory
```shell
rm -r DIRECTORY-NAME
```
## shell output
return to command line from shell output
```shell
:q
```
## apt
update apt package list (to obtain information on newest versions)
```shell
sudo apt update
```
fetch newest versions of apt packages and remove packages if necessary
```shell
sudo apt full-upgrade
```
remove obsolete packages after upgrade or removal
```shell
sudo apt autoremove
```
install apt packages on the system
```shell
sudo apt install PACKAGE-NAME
```
remove apt packages from the system
```shell
sudo apt remove PACKAGE-NAME
```
## snap
update snap packages
```shell
sudo snap refresh
```
install snap packages on the system
```shell
sudo snap install PACKAGE-NAME
```
remove snap packages from the system
```shell
sudo snap remove PACKAGE-NAME
```
## ufw
enable ufw
```shell
sudo ufw enable
```
deny incoming traffic
```shell
sudo ufw default deny incoming
```
allow outgoing traffic
```shell
sudo ufw default allow outgoing
```
check status
```shell
sudo ufw status verbose
```
## ClamAV
update signature databases
```shell
sudo freshclam
```
kill freshclam started by ClamAV daemon before manual freshclam
```shell
sudo killall freshclam
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
## shutdown and restart
shutdown in under a minute
```shell
shutdown -h
```
restart in under a minute
```shell
shutdown -r
```
cancel scheduled shutdown/restart
```shell
shutdown -c
```