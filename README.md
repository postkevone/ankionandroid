**YouTube Tutorial**

[![youtube tutorial](https://img.youtube.com/vi/0RNs27woiJ4/0.jpg)](https://www.youtube.com/watch?v=0RNs27woiJ4)
***
・Install termux
・Setup the storage folders and give storage permission
```following
termux-setup-storage
```
・Update all the termux packages installed (type 'Y' if requested)
```
apt update && apt upgrade
```
・Install the andronix app
・Install modded manjaro (it costs 2$ but this tutorial should also work with free version)
・Paste the token into Termux and wait until the download is completed
・Start androjaro
```
./start-androjaro.sh
```
・Start the VNC Server
```
vncserver-start
```
***
・Install "VNC Viewer" from the play store
・Open it, create a new connection on localhost and give it a name
```
localhost:1
name
```
・Start androjaro and adjust your display settings
***
・From the file manage find and open the following file:
```
/etc/pamac.d/mirrorlist
```
・Delete everything and paste the following link:
```
http://manjaro-arm.moson.eu/arm-stable/$repo/$arch
```
・Open the terminal and update all the pacman packages (takes up to 3/4 hours depending on your downloading speed)
```
sudo pacman -Syu && sudo pacman-key --init && sudo pacman-key --populate && sudo pacman -Syu
```
***
・Install mplayer
```
sudo pacman -S mplayer
```
・Download ffmpeg from https://archlinuxarm.org/packages/aarch64/ffmpeg
・Download noto fonts for asian characters (chinese, japanese, korean) (optional) https://archlinuxarm.org/packages/any/noto-fonts-cjk
・Download anki arm version https://archlinuxarm.org/packages/any/anki
・Install the packages by typing (drag the downloaded file into the terminal, it will automatically generate the path directory)
```
sudo pacman -U filename
```
・You can now access anki from the Educational Software folder
・When you're done, remember to always terminate the vncserver by typing:
```
vncserver-stop
```
