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

## Si pb avec mapping de l'écran

`xsetwacom --list devices` pour avoir la liste des appareils et leurs id.
`xrandr liveactivemonitors` pour avoir la liste des écrans actifs

`xsetwacom --set <nom du stylet ou id> MapToOutput <nom de l'écran>` pour mapper le stylet à l'écran de la tablette [source](https://askubuntu.com/a/1082433)

si ça ne fonctionne pas (j'ai eu l'erreur "Unable to find an output <nom de l'écran>." apparemment car j'ai une carte Nvidia) utiliser `xsetwacom --set <nom de stylet ou id> MapToOutput HEAD-1` [source](https://doc.ubuntu-fr.org/wacom#dual_screen_ou_mapper_la_tablette_sur_un_seul_ecran)

utiliser le `'<nom du stylet>'` peut être mieux que son `<id>` car ce dernier peut changer (j'ai des pb de déconnexion USB)
