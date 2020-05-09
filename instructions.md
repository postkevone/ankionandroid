**youtube tutorial**

[![youtube tutorial](https://img.youtube.com/vi/0RNs27woiJ4/0.jpg)](https://www.youtube.com/watch?v=0RNs27woiJ4)
***
install termux, then type in the terminal the following command
```
termux-setup-storage
```
give storage permission

type in the terminal the following command
```
apt update && apt upgrade
```
type y then exit

install andronix

install modded manjaro (2$ but should work with free version as well)

it will automatically open termux, paste the token and the download should start

when it finishes downloading type 
```
./start-androjaro.sh
```
```
vncserver-start
```
***
install vnc viewer

create a new connection
```
localhost:1
name
```

adjust display settings to match with your device
***
open the following file
```
/etc/pamac.d/mirrorlist
```
replace every server link with
```
http://manjaro-arm.moson.eu/arm-stable/$repo/$arch
```
type the following command in the terminal to update (takes time)
```
sudo pacman -Syu && sudo pacman-key --init && sudo pacman-key --populate && sudo pacman -Syu
```
***
download ffmpeg

https://archlinuxarm.org/packages/aarch64/ffmpeg

install by typing
```
sudo pacman -U file
```
(instead of "file" drag the download archive to the terminal, it will automatically generate the path directory)
***
install mplayer
```
sudo pacman -S mplayer
```
***
install chinese, japanese, korean font (optional)

https://archlinuxarm.org/packages/any/noto-fonts-cjk
```
sudo pacman -U file
```
***
install anki arm

https://archlinuxarm.org/packages/any/anki
```
sudo pacman -U file
```

you can find anki in the educational software
***
remember to always exit and terminate the vncserver by typing after androjaro has started
```
vncserver-stop
```
