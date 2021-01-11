---
layout: none
title: Guide du créatif libre

krita-use: Dessin et peinture numérique.
krita-image: img/krita.jpg
krita-description: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed sed volutpat nunc, ut accumsan lectus. Nunc id suscipit quam, a maximus lectus. Pellentesque ultricies purus justo, vel malesuada tortor sagittis ut. Mauris tincidunt sem ut feugiat interdum. Etiam molestie interdum nulla nec sollicitudin.


---

<DOCTYPE html>
<html lang="fr">
<head>
    <link rel="stylesheet" type="text/css" href="stylesheet.css">
    <title>{{ page.title }}</title>
</head>
<body>
    <div id='navbar'>
        <a href="#navbar">Home</a>
        <a href="#krita">Krita</a>
        <a href="#blender">Blender</a>
        <a href="#inkscape">Inscape</a>
        <a href="#scribus">Scribus</a>
        <a href="#kdenlive">Kdenlive</a>
        <a href="#godot">Godot</a>
        <a href="#audacity">Audacity</a>
    </div>

    <div class='container' id='krita'>
        <h1>Krita</h1>
        <h2> {{ page.krita-use }}</h2>
        <img src="{{ page.krita-image }}" alt="image Krita" width="300" height="200">
        <p> {{ page.krita-description }}</p>
        <a href="blank">en apprendre plus</a>
        <p>Voir aussi : <a href="blank">GIMP</a>.</p>
        <p>Voir aussi 2 : {{ page.krita-link }}</p>

    </div>

    <div class='container' id='blender'>
        <h1>Blender</h1>
        <h2>Modélisation 3D, animation 2D & 3D, montage vidéo et bien plus.</h2>
        <img src="img/blender.jpeg" alt="image Blender" width="300" height="200">
        <p>Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Sed egestas viverra lectus, nec finibus felis tincidunt eget. Sed id augue tellus. </p>
        <a href="blank">en apprendre plus</a>

    </div>

    <div class='container' id='inkscape'>
        <h1>Inkscape</h1>
        <h2>Dessin vectoriel et illustration.</h2>
        <img src="img/inkscape.png" alt="image Inkscape" width="300" height="200">
        <p>Vestibulum venenatis urna et dignissim luctus. Morbi bibendum lorem ac eros ullamcorper iaculis. Nullam ut aliquam ipsum. Aliquam pellentesque sapien id leo imperdiet lacinia. Nam porta sapien neque, ac tempus sapien facilisis at.</p>
        <a href="blank">en apprendre plus</a>

    </div>

    <div class='container' id='scribus'>
        <h1>Scribus</h1>
        <h2>Mise en page.</h2>
        <img src="img/scribus.png" alt="image Scribus" width="300" height="200">
        <p>Donec et rutrum risus. Fusce tellus tortor, rutrum ut mattis ut, egestas non sapien. In imperdiet, ipsum et varius volutpat, est risus dictum dolor, a ornare erat velit quis mi. Curabitur lorem lectus, fringilla ut velit eget, condimentum condimentum neque. Aenean condimentum auctor odio, nec imperdiet orci cursus eget.</p>
        <a href="blank">en apprendre plus</a>

    </div>

    <div class='container' id='kdenlive'>
        <h1>Kdenlive</h1>
        <h2>Montage vidéo.</h2>
        <img src="img/kdenlive.jpeg" alt="image Kdenlive" width="300" height="200">
        <p>Phasellus id ex venenatis, tempus ipsum vitae, fermentum purus. Praesent finibus diam pellentesque urna vulputate pharetra. </p>
        <a href="blank">en apprendre plus</a>
        <p>Voir aussi : <a href="blank">Blender (VSE)</a>, <a href="blank">OpenShot</a>
    </div>

    <div class='container' id='godot'>
        <h1>Godot</h1>
        <h2>Moteur de jeux 2D & 3D.</h2>
        <img src="img/godot.jpeg" alt="image Godot" width="300" height="200">
        <p>Donec eget pretium nisl. Phasellus magna est, blandit feugiat elit vel, accumsan congue neque. Mauris dictum eget eros id bibendum. Sed sollicitudin nulla purus, a dictum libero consectetur in. Praesent et sollicitudin ante, interdum sollicitudin purus.</p>
        <a href="blank">en apprendre plus</a>
        <p>Voir aussi : <a href="blank">LÖVE (2D)</a>
    </div>

    <div class='container' id='audacity'>
        <h1>Audacity</h1>
        <h2>Enregistrement et édition audio.</h2>
        <img src="img/audacity.png" alt="image Audacity" width="300" height="200">
        <p>Vestibulum sed imperdiet urna. Maecenas sit amet magna quam. Suspendisse fermentum tempor urna, ac lacinia lorem auctor vitae. Aenean blandit nunc in diam finibus tincidunt. Fusce id dui urna. Praesent tempus elementum eros ac tincidunt. </p>
        <a href="blank">en apprendre plus</a>

    </div>
</body>
