# Ubuntu 18.10 Post Install

## 1. Update ubuntu with latest packages and upgrades
$ sudo apt-get update && sudo apt-get upgrade

## 2. Installing Google Chrome
### Using PPA

$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add - \
$ sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list' \
$ sudo apt-get update \

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
$ sudo add-apt-repository universe \
$ sudo apt install gnome-tweak-tool

## 7. Enable canonical updates and install additional drivers

## 8. Install Archive applications
$ sudo apt-get install unrar zip unzip p7zip-full p7zip-rar rar

## 9. Install Wine
$ sudo apt-get install wine winetricks

## 10. Install different desktop environment
### Cinnamon
$ sudo apt-get install cinnamon-desktop-environment
### Mate
$ sudo apt-get install ubuntu-mate-desktop
### KDE
$ sudo apt install tasksel \
$ sudo tasksel install kubuntu-desktop \
$ sudo apt install sddm \
$ sudo dpkg-reconfigure sddm 

## 11. Install Nodejs
$ sudo apt-get install nodejs \
$ sudo apt-get install npm

## 12. Install docker
$ sudo apt-get install \\
    apt-transport-https \\
    ca-certificates \\
    curl \\
    gnupg-agent \\
    software-properties-common \
    
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - \
$ sudo add-apt-repository \\
     "deb [arch=amd64] https://download.docker.com/linux/ubuntu \\
     $(lsb_release -cs) \\
     stable" \
$ sudo apt-get update \
$ sudo apt-get install docker-ce docker-ce-cli containerd.io
### Install specifc version
#### List available versions
$ apt-cache madison docker-ce
#### Install specific version
$ sudo apt-get install docker-ce=<VERSION_STRING> docker-ce-cli=<VERSION_STRING> containerd.io
