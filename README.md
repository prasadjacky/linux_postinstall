# Ubuntu 18.10 Post Install

## 1. Update ubuntu with latest packages and upgrades
$ sudo apt-get update && sudo apt-get upgrade

## 2. Installing Google Chrome
### Using PPA

$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
$ sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
$ sudo apt-get update

#### Chrome Stable
$ sudo apt-get install google-chrome-stable
#### Chrome Beta
$ sudo apt-get install google-chrome-beta

## 3. Install Gnome shell extensions
$ sudo apt install chrome-gnome-shell

## 4. Install media codecs
$ sudo apt install ubuntu-restricted-extras

## 5. Install apps from Software center
- VLC
- VS Code
- Termius
- Steam

## 6. Install Gnome tweaks
$ sudo add-apt-repository universe
$ sudo apt install gnome-tweak-tool

## 7. Enable canonical updates and install additional drivers

## 8. Install Archive applications
$ sudo apt-get install unrar zip unzip p7zip-full p7zip-rar rar
