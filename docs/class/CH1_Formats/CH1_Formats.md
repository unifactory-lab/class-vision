# Chapitre 1 : Formats d'image

## Qu'est-ce qu'une image ?
En informatique, les images utilisées sont des "images matricielles". Des "cartes de points" ou "bitmap" en anglais. La carte de points est une grille ou un pavage, dont chaque élément est un carré appelé "pixel". Chaque pixel contient, dans la majorité des cas, une valeurs comprise entre 0 et 255 (parfois normalisé entre 0 et 1).

Attention, il est à noter que le terme anglais "bitmap" peut designer aussi un tableau de donnée booléen, ou similairement, une image binarisée.

<img class="img-no-border" src="../DigitalPicture.jpg" alt="Représentation d'une image bitmap">

*Exemple d'image matricielle. L’auteur n’a pas pu être identifié automatiquement. Il est supposé qu'il s'agit de : Ivanoff~commonswiki (étant donné la revendication de droit d’auteur). — La source n’a pas pu être reconnue automatiquement. « Travail personnel » supposé (étant donné la revendication de droit d’auteur)., CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=2012046*

## Images multicouches
Avec une valeur unique par pixel, les images représentées sont en niveau de gris. Afin de palier à ce problème, les images couleurs sont constituées de plusieurs couches. Cela permet de stocker plusieurs valeurs par pixel.

<img class="img-no-border" src="../Rgb-raster-image.png" alt="Le smiley situé dans le coin supérieur gauche est une image matricielle. Lorsqu'on l'agrandit, les pixels apparaissent sous forme de carrés. En l'agrandissant encore davantage, on peut analyser chaque pixel, dont la couleur résulte de la combinaison des valeurs de rouge, de vert et de bleu.">

*Le smiley situé dans le coin supérieur gauche est une image matricielle. Lorsqu'on l'agrandit, les pixels apparaissent sous forme de carrés. En l'agrandissant encore davantage, on peut analyser chaque pixel, dont la couleur résulte de la combinaison des valeurs de rouge, de vert et de bleu. By Gringer - Own work, CC0, https://commons.wikimedia.org/w/index.php?curid=17126728*

Les images couleurs sont constituées de trois couches. Il existe plusieurs façon d'encoder les couleurs, qui peuvent être plus ou moins pratiques en fonction des usages.

- RGB
    - R/RED : Niveau de rouge
    - G/GREEN : Niveau de vert
    - B/BLUE : Niveau de bleu

<img class="img-no-border" src="../RGB_color_solid_cube.png" alt="Le modèle de couleur RVB représenté sur un cube. L'axe horizontal x correspond aux valeurs de rouge, qui augmentent vers la gauche ; l'axe vertical y correspond aux valeurs de bleu, qui augmentent vers le bas à droite ; et l'axe vertical z correspond aux valeurs de vert, qui augmentent vers le haut. L'origine, de couleur noire, correspond au sommet masqué à la vue.">

*Le modèle de couleur RVB représenté sur un cube. L'axe horizontal x correspond aux valeurs de rouge, qui augmentent vers la gauche ; l'axe vertical y correspond aux valeurs de bleu, qui augmentent vers le bas à droite ; et l'axe vertical z correspond aux valeurs de vert, qui augmentent vers le haut. L'origine, de couleur noire, correspond au sommet masqué à la vue. By SharkD - Own work Source-code available at the POV-Ray Object Collection., CC BY-SA 4.0, https://commons.wikimedia.org/w/index.php?curid=3375025*

<div class="grid cards" markdown>

-   __Couches RGB__

    <img class="img-no-border-small" src="../separate_red.png" alt="Composante rouge.">
    <img class="img-no-border-small" src="../separate_green.png" alt="Composante verte.">
    <img class="img-no-border-small" src="../separate_blue.png" alt="Composante bleue.">
    <img class="img-no-border-small" src="../photo.jpg" alt="Photo originale.">

</div>

- HSV
    - H/HUE :Teinte
    - S/SATURATION : Saturation
    - V/VALUE : Valeur

<img class="img-no-border" src="../HSV_color_solid_cylinder_saturation_gray.png" alt="Cylindre TSV des couleurs.">

*Cylindre TSV des couleurs. Par HSV_color_solid_cylinder.png: SharkDderivative work: SharkD  Talk — HSV_color_solid_cylinder.png, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=9801673*

<div class="grid cards" markdown>

-   __Couches RGB__

    <img class="img-no-border-small" src="../separate_hue.png" alt="Teinte.">
    <img class="img-no-border-small" src="../separate_sat.png" alt="Saturation.">
    <img class="img-no-border-small" src="../separate_val.png" alt="Valeur.">
    <img class="img-no-border-small" src="../photo.jpg" alt="Photo originale.">

</div>
- Lan
    - L/Lightness : Clarté
    - a & b : écart de couleur avec un gris de même clarté.

<img class="img-no-border" src="../CIELAB_color_space_top_view.png" alt="Nuage de points des couleurs optimales (chroma maximal théorique des surfaces) dans l'espace CIE Lab, vue de dessus.">

*Nuage de points des couleurs optimales (chroma maximal théorique des surfaces) dans l'espace CIE Lab, vue de dessus. By Holger kkk Everding - Own work, CC BY-SA 4.0, https://commons.wikimedia.org/w/index.php?curid=38366968*

Une quatrième couche, correspondant à la transparence, est parfois ajouté dans certains formats comme le ".png".

## Caractéristiques des images

### Ratio d'aspect
Le ratio d'aspect est le rapport entre la longueur et la largeur de l'image. Par exemple, la majorité des écrans d'ordinateur actuel ont un format 16:9 (1.78:1). C'est à dire qui si l'image est constituée de 16 unités en longueur, elle est contituée de 9 unités en largeur.

<img class="img-no-border" src="../Filmaspectratios.png" alt="Comparaison de plusieurs formats d'image de films, les hauteurs des images étant forcées d'être identiques.">

*Comparaison de plusieurs formats d'image de films, les hauteurs des images étant forcées d'être identiques. By Original: Tyhart87 Vector: Andresconrado - Filmaspectratios.jpg, Public Domain, https://commons.wikimedia.org/w/index.php?curid=7555009*

### Définition
La définition d'une image est constitué du nombre de pixel horizontaux et verticaux de l'image. Ce terme est souvent interchangé avec la résolution de l'image.

### Résolution
La résolution d'une image correspond, lorsqu'elle est imprimée sur un support physique, au nombre de pixel par unité de longueur. Elle est souvent exprimée en pixel par pouce (PPP, ou dot per inch, dpi, en anglais). Des résolutions classiques sont 300 dpi et 600 dpi.

### Système de coordonnée
Les images utilisent un système de coordonées particulier. C'est un système à deux dimensions, nommées (u,v), (U,V), (x,y) ou encore (X,Y). Le système prend son origine en haut à gauche de l'image avec le pixel de coordonnées (1,1). La première coordonnée augmente en se déplaçant vers la droite, alors que la deuxième augmente en se déplaçant vers le bas.

<img class="img-no-border" src="../dtv32.jpg" alt="Photo d'une main dans un salon sur laquelle est appliqué un algorithme de détection des features. Les coordoonées des coins de l'images et de certaines features sont montrées.">

*Photo d'une main dans un salon sur laquelle est appliqué un algorithme de détection des features. Les coordoonées des coins de l'images et de certaines features sont montrées. La définition de l'image est 256x256. Le pixel d'origine a donc pour coordonnée (1,1), le pixel à l'opposée de l'image, en bas à droite, a pour coordonnée (256,256)*

Souvent, deux systèmes (u,v) et (x,y) sont différenciés. Bien qu'ils aient la même orientation, le système (u,v) colle à la description faîtes précedemment. Alors que le système (x,y) prends sont origine au niveau du "centre optique" de la caméra qui a capturé l'image, et ses coordonnées sont sans unités ou dans une unité de longueur comme les milimètres.

<!-- ## Formats d'images, introduction à la compression

### Compression avec et sans perte

### Les différents formats d'image -->