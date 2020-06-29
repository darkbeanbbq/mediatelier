# Setup de la tablette Huion Kamvas 13 (2020)

~ fonctionne out of the box avec xorg

installer driver digimend la rend visible/compatible avec xsetwacom


obtenir le nom de la tablette avec  `xsetwacom list`, moi j'ai eu "Tablet Monitor Pad pad"

bind les touches avec `xsetwacom set "NOM_DE_LA_TABLETTE" Button NUMÉRO "key TOUCHE"` comme ceci :
```
xsetwacom set "Tablet Monitor Pad pad" Button 1 "key 1"
xsetwacom set "Tablet Monitor Pad pad" Button 2 "key 2"
xsetwacom set "Tablet Monitor Pad pad" Button 3 "key 3"

xsetwacom set "Tablet Monitor Pad pad" Button 8 "key shift ="
xsetwacom set "Tablet Monitor Pad pad" Button 9 "key -"

xsetwacom set "Tablet Monitor Pad pad" Button 10 "key 4"
xsetwacom set "Tablet Monitor Pad pad" Button 11 "key 5"
xsetwacom set "Tablet Monitor Pad pad" Button 12 "key 6"
```

"key shift =" = "+"
car key = la touche physique et pas le caractère, donc pour faire un "+" il faut physiquement appuyer sur "shift"

ctrl z,



## Krita keys

```
#!/bin/bash

DEVICE="Tablet Monitor Pad pad"

xsetwacom set "$DEVICE" Button 1 "key 5" # reset rotation
xsetwacom set "$DEVICE" Button 2 "key ctrl z"
xsetwacom set "$DEVICE" Button 3 "key e" # eraser

xsetwacom set "$DEVICE" Button 8 "key shift ="
xsetwacom set "$DEVICE" Button 9 "key -"

xsetwacom set "$DEVICE" Button 10 "key t" # transform
xsetwacom set "$DEVICE" Button 11 "key ctrl"
xsetwacom set "$DEVICE" Button 12 "key shift"
```


## lancé au démarrage

sauvegarder son script xsetwacom.sh dans ".local/bin" (par exemple) et le rendre exécutable `chmod +x $HOME/.local/scripts/xsetwacom.sh` (ou via clic droit)

lancer "Application au démarrage" via le launcher ou `gnome-session-properties` et ajouter le script.


[source](https://github.com/linuxwacom/xf86-input-wacom/wiki/Tablet-Configuration-1:-xsetwacom-and-xorg.conf)
