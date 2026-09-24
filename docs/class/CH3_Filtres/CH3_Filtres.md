# Chapitre 3 : Morphologie et filtres

## Binarisation

L'histogramme d'une image est la représentation graphique de la distribution des pixels de l'image en fonction de leur valeur. En abscisse se trouves toutes les valeurs possibles pour les pixels : classiquement de 0 à 255. En ordonnée, le nombre de pixels qui ont pour valeur celle indiquée en abscisse.

<img class="img-no-border" src="../Image_and_histogram.png" alt="Une image et son histogramme, avec le pic correspondant au blanc (neige et nuages).">

*Une image et son histogramme, avec le pic correspondant au blanc (neige et nuages). Par Mer_de_Glace_hiver.jpg: Syleniusderivative work: Sylenius (talk) — Mer_de_Glace_hiver.jpg, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=11525103*

De nombreux algorithmes agissent, d'un point de vue théorique, sur l'histogramme de l'image. Bien qu'en pratique, ces algorithmes agissent directement sur l'image.

La binarisation est l'algorithme d'histogramme le plus connu. Il rempli plusieurs fonctions :

 - Séparation de différentes partie d'une image.
 - Création de masque.
 - Suppression des informations inutiles au traitement.

L'algorithme fonctionne ainsi : un seuil est choisi entre la valeur minimum et la valeur maximum possibles des pixels. De 0 à 255 dans la majorité des cas. Ensuite, tous les pixels dont la valeur est en dessous du seuil sont passés à la valeur minimum, tous les pixels dont la valeur est au dessus du seuil passent à la valeur maximum.


<img class="img-no-border" src="../Angelica_pollen_grain_image_binarization.jpg" alt="Binarisation d'une image de grain de pollen. a gauche : image originale. A droite : image binaire.">

*Binarisation d'une image de grain de pollen. a gauche : image originale. A droite : image binaire. Par Ханжина Наталья Евгеньевна — Travail personnel, CC BY-SA 4.0, https://commons.wikimedia.org/w/index.php?curid=45015281*

Il existe des variantes plus ou moins complexes de la binarisation, permettant d'avoir des résultats plus adaptés en fonction des cas d'usage. Une variante connu est la méthode d'Otsu, qui permet de tenir compte des variations de luminosité locale dans l'image.

## Opération morphologique

<img class="img-no-border" src="../DilationErosion.png" alt="Une forme (en bleu), sa dilatation morphologique (en vert), et son érosion morphologique (en jaune) par un élément structurant en forme de diamant.">

*Une forme (en bleu), sa dilatation morphologique (en vert), et son érosion morphologique (en jaune) par un élément structurant en forme de diamant. Par Renato Keshet — created by the user, Domaine public, https://commons.wikimedia.org/w/index.php?curid=4413072*

Les opérations morpholiques s'appliquent à des images binarisés, elle permettent, la plupart du temps, de corriger les défauts présents sur les images binarisés. Les opérations seront illustrées grâce à l'image suivante :

<img class="img-no-border" src="../Illustration_morpho.png" alt="Image originale (en noir : l'objet ; en blanc : le fond).">

*Image originale (en blanc : l'objet ; en noir : le fond). Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600427*

Les opérations morphologiques sont effectuées par convolution.

### Dilatation

Si au moins un pixel en dessous du noyau est à la valeur maximal, alors le pixel résultant sera à la valeur maximale. La dilatation a pour effet d'élargir les zones blanches de l'image.

<img class="img-no-border" src="../Illustration_dilatation.png" alt="Dilatation par un carré 3x3 : les pixels blancs et gris font partie de l'ensemble résultant.">

*Dilatation par un carré 3x3 : les pixels blancs et gris font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600447*

### Erosion

L'érosion peut-être considéré comme l'inverse de la dilatation. Le pixel résultant est à la valeur maximale si et seulement si tous les pixels sous le noyaux sont à la valeur maximale, sinon, il est érodé (mis à la valeur minimale).

<img class="img-no-border" src="../Illustration_erosion.png" alt="Érosion par un carré 3x3 : seuls les pixels blancs font partie de l'ensemble résultant.">

*Érosion par un carré 3x3 : seuls les pixels blancs font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600436*

### Fermeture

La fermeture est l'application d'une érosion suivie d'une dilatation. Elle peut permettre, entre autre, de réduire le bruit sur les parties blanches de l'image.

<img class="img-no-border" src="../Illustration_fermeture.png" alt="Fermeture par un carré 3×3 : les pixels blancs et gris font partie de l'ensemble résultant.">

*Fermeture par un carré 3×3 : les pixels blancs et gris font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600457*

### Ouverture

L'ouverture est l'application d'une dilatation suivie d'une érosion. Elle peut permettre, entre autre, de réduire le bruit sur les parties noires de l'image.

<img class="img-no-border" src="../Illustration_ouverture.png" alt="Ouverture par un carré 3×3 : seuls les pixels blancs font partie de l'ensemble résultant">

*Ouverture par un carré 3×3 : seuls les pixels blancs font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600455*

## Filtres

### Détection des bords


<img class="img-no-border" src="../Intensity_image_with_gradient_images.png" alt="On the left, an intensity image of a cat. In the center, a gradient image in the x direction measuring horizontal change in intensity. On the right, a gradient image in the y direction measuring vertical change in intensity. Gray pixels have a small gradient; black or white pixels have a large gradient.">

*On the left, an intensity image of a cat. In the center, a gradient image in the x direction measuring horizontal change in intensity. On the right, a gradient image in the y direction measuring vertical change in intensity. Gray pixels have a small gradient; black or white pixels have a large gradient. By Njw000 - Own work, Public Domain, https://commons.wikimedia.org/w/index.php?curid=10588443*

## Détection des lignes

### Transformée de Hough

## Ressources

📖 [OpenCV - Histogramme](https://docs.opencv.org/4.13.0/d1/db7/tutorial_py_histogram_begins.html)

📖 [OpenCV - Binarisation](https://docs.opencv.org/4.13.0/d7/d4d/tutorial_py_thresholding.html)

📖 [OpenCV - Opération morphologique](https://docs.opencv.org/4.13.0/d9/d61/tutorial_py_morphological_ops.html)

📖 [OpenCV - Gradients](https://docs.opencv.org/4.13.0/d5/d0f/tutorial_py_gradients.html)

📖 [OpenCV - Transformée de Hough](https://docs.opencv.org/4.13.0/d6/d10/tutorial_py_houghlines.html)

📖 [OpenCV - Canny](https://docs.opencv.org/4.13.0/da/d22/tutorial_py_canny.html)