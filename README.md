anki 2.1.15 arm on android (termux)

install termux
storage permission
termux-setup-storage
apt update && apt upgrade

install andronix
install modded manjaro (2$)
(should work with free version as well)

./start-androjaro.sh
vncserver-start
vncserver-stop

install vnc viewer
localhost:1

adjust display settings

update pacman
/etc/pamac.d/mirrorlist replace server link with
http://manjaro-arm.moson.eu/arm-stable/$repo/$arch/
sudo pacman -Syu && sudo pacman-key --init && sudo pacman-key --populate && sudo pacman -Syu

install pamac
sudo pacman -Syu pamac-qt

install ffmpeg
https://archlinuxarm.org/packages/aarch64/ffmpeg
sudo pacman -U file

install mplayer
sudo pacman -S mplayer

install chinese, japanese, korean font (optional)
https://archlinuxarm.org/packages/any/noto-fonts-cjk
sudo pacman -U file

install anki arm
https://archlinuxarm.org/packages/any/anki
sudo pacman -U file
