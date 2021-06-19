# Créer des visuels à découper avec Krita et Inkscape

pour un meilleur résultat il faut :
- savoir comment la machine fonctionne (découpe le tracé, plus il grand/long/détaillé plus c'est long à découper et préparer)
- avoir des bases en dessin vectoriel / vectorisation d'image (image bien contrasté ou en N&B, notion de nœud, fond vs. contour)

**comment changer la langue ?**

## Créer son dessin avec Krita
- *découverte de l'interface* (barre d'outils, barre menu, sélecteur de couleurs, préférences d'outils, calques, préréglages de brosses,)
- *navigation et raccourcis clavier* (zoom, pan, taille brosses, etc.)

- choisir une brosse (pinceau) pas trop stylisée, ex: `b)_Basic-1` ou `b)_Basic-5_Size`
- faire son dessin en noir et blanc
- l'exporter au format .png

## Vectoriser son dessin avec Inkscape
- *découverte de l'interface* (barre d'outils, menu contextuel de l'outil, panneaux, barre de menu bis, palette en bas, magnétisme)
- *navigation et raccourcis clavier* (zoom, pan, outils, etc.)
- *concept du dessin vectoriel* (nœuds, chemins, courbe de bézier, fond/contour)

- importer le dessin (glisser-déposer), cliquer OK sur la fenêtre d'importation
- vectoriser le dessin, chemin > vectoriser un objet matriciel (ctrl alt B)
  - par seuil de luminosité, jouer avec le seuil, mettre à jour, puis valider quand c'est bon (+ fermer fenêtre)
  - séparer image de son double vectorisé
- nettoyer si besoin le tracé avec l'outil sélecteur de nœuds

- contour en couleur pour voir ce que la machine voit

- supprimer tout ce que vous ne voulez pas découper
- sauvegarder au format SVG simple (pour éviter les pb, mais SVG Inkscape devrait aussi marcher)
