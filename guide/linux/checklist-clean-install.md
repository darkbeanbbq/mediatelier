# Que faire quand je fait une installation propre de Linux

## Avoir fait un backup

Mes grands dossiers dans `$HOME`

Mais aussi ne pas oublier des dossiers comme le `$HOME/.fonts` ou `$HOME/.config`

## Installation de programmes

### Les indispensables

- Firefox
- Atom (télécharger hanspell-fr pour la correction en français)
- Inkscape
- Krita
- Scribus
- Blender
- Godot
- VLC (télécharger libdvdcss pour lecture de DVD)
- Audacity

### Utilitaires

- OBS Studio
LibreOffice
FontForge
- PureRef
- Etcher
- Peek
- gnome-tweaks

Oracle VM (pas encore de verison pour 20.04)
Ruby (pour Jekyll)
Python
- neofetch

### Communication et réseaux sociaux

- Thunderbird
- Slack
- Discord
Riot
TeamViewer


### Autres

- Steam
Dolphin Emulator
Kdenlive
- MarkText
- gnome-sushi
- pop-shell


## Gestion des AppImages
les stocker dans $Home/.local/bin

### Création de fichiers .desktop
à créer et stocker dans $Home/.local/share/applications

```
[Desktop Entry]
Name=Godot Engine
Comment=Free and Open Source 2D and 3D Game Engine
Terminal=false
Type=Application
Categories=Development;IDE;
Keywords=game;engine;ide;
Exec=/home/darkbean/.local/bin/Godot_v3.2.1-stable_x11.64
Icon=/home/darkbean/.local/bin/godot.png
```

## Avoir un ç quand on fait ' + c
