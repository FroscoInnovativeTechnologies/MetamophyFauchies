# MetamophyFauchies
A wallpaper engine like application for xorg WMs

to build this app to an installable DEB file :
```
  chmod +x metamorphy-fauchies_1.2_all/DEBIAN/postinst
  chmod +x metamorphy-fauchies_1.2_all/usr/bin/metamorphy-fauchies
  dpkg -b metamorphy-fauchies_1.2_all/
```

the default config.txt contains
```
  #This is a sample config
  #place this file in $HOME/.config/metamorphy-fauchies/ under the name config.txt

  #provider sets the background source
  #0 for local $HOME/Pictures/metamorphy-fauchies/
  #1 for nekos.py
  #2 for bing wallpapers
  #3 for picsum
  provider 1

  #style is a nekos.py exclusive parameter
  #0 for fox girl
  #1 for cat girl
  style 1

  #interval is the time between each update set in seconds
  interval 30

  #this section is for picsum specific settings
  #set an image to GrayScale 0 for False and 1 for True
  gray 0

  #add blur to an image 0 for False and 1 for True
  blur 0

  #the ammount of blur in PX
  blurpx 1

  #the height of the images in PX
  height 1280

  #the width of the images in PX
  width 800
```

refer to the `config.sample.txt` file for more info
config.txt should be placed in `~/.config/metamorphy-fauchies/`

local wallpaper directory is located in `~/Pictures/metamorphy-fauchies/`

it can be ran from terminal or your WM autostart script by typing `metamorphy-fauchies`

more info soon
