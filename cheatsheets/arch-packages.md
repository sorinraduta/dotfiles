## Arch packages
##### Update pacman packages
`pacman -Suy --noconfirm`

##### Install make utils
```
pacman -S --noconfirm \
git \
binutils \
make \
gcc \
fakeroot
```

##### Install yay
```
cd /tmp
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
cd ..
rm -rf yay
```

#### Install packages
`yay -S --noconfirm \`

##### X Server
```
#xorg-server \
#xorg-apps \
#xorg-xinit \
xorg-xsetroot \
xorg-xinput \
xorg-server-xephyr \
xorg-xev \
xorg-xlsfonts \
xorg-xfontsel \
```

##### Display manager
```
#lightdm \
#lightdm-gtk-greeter \
#lightdm-webkit2-greeter \
lightdm-webkit-theme-sequoia-git \
```

##### Desktop enviroment
```
i3-gaps \
gnome \
gnome-extra \
```

##### Development
```
code \
nodejs \
yarn \
go \
nodejs \
npm \
mariadb \
docker \
docker-compose \
mycli \
python \
python2 \
python-pip \
dbeaver \
ansible \
```

##### Rice
```
chromium \
zsh \
feh \
dunst \
kitty \
ranger \
rofi \
polybar \
picom \
volnoti \
deepin-screenshot \
network-manager-applet \
redshift \
gnome-icon-theme \
ttf-hack \
ttf-font-awesome \
```

##### Network
```
openvpn \
xl2tpd \
strongswan \
```

##### Utils
```
dotdrop \
playerctl \
curl \
wget \
man \
jq \
imagemagick \
fortune-mod \
cowsay \
vim \
arandr \
cronie \
lm_sensors \
acpi \
cmatrix \
neofetch \
wmctrl \
moc-pulse \
tty-clock \
pacman-contrib \
projectlibre \
unclutter \
dialog \
fping \
```

##### X Utils
```
xclip \
xdotool \
xautolock \
```

##### Display applications
```
gimp \
slack-desktop \
postman-bin
rambox \
chromium \
lastpass
```

##### Install oh my zsh
```
sh -c "$(wget -O- https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
chsh -s $(which zsh)
homectl update rappy --shell=/usr/bin/zsh
```

##### MariaDB
`mariadb-install-db --user=mysql --basedir=/usr --datadir=/var/lib/mysql`

##### Enable system services
```
sudo systemctl enable lightdm
sudo systemctl enable light-locker
sudo systemctl enable mariadb
sudo systemctl enable strongswan
sudo systemctl enable docker
```

##### Enable user services
```
systemctl --user enable picom
systemctl --user enable redshift
systemctl --user enable unclutter
systemctl --user enable volnoti
systemctl --user enable polybar@bottom.timer
systemctl --user enable polybar@top.timer
```

##### Sync date and time
```
timedatectl set-timezone Europe/Bucharest
timedatectl set-ntp true
sudo systemctl restart systemd-timedated
sudo systemctl restart systemd-timesyncd
```

##### Login on websites
```
chromium \
https://accounts.google.com \
https://trello.com/login \
https://github.com/login \
https://login.yahoo.com \
https://login.yahoo.com \
https://login.yahoo.com \
https://ufcfightpass.com/login \
https://discord.com/login \
https://linkedin.com/login \
https://instagram.com \
https://slack.com/signin \
https://id.atlassian.com/login \
https://netflix.com/login \
https://reddit.com/login \
https://twitter.com/login \
https://web.whatsapp.com \
chrome://flags/#enable-native-notifications
```
