# Chapitre 3 : Morphologie et filtres

## Binarisation

📖 [OpenCV - Histogramme](https://docs.opencv.org/4.13.0/d1/db7/tutorial_py_histogram_begins.html)

<img class="img-no-border" src="../Image_and_histogram.png" alt="Une image et son histogramme, avec le pic correspondant au blanc (neige et nuages).">

*Une image et son histogramme, avec le pic correspondant au blanc (neige et nuages). Par Mer_de_Glace_hiver.jpg: Syleniusderivative work: Sylenius (talk) — Mer_de_Glace_hiver.jpg, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=11525103*

📖 [OpenCV - Binarisation](https://docs.opencv.org/4.13.0/d7/d4d/tutorial_py_thresholding.html)

<img class="img-no-border" src="../Angelica_pollen_grain_image_binarization.jpg" alt="Binarisation d'une image de grain de pollen. a gauche : image originale. A droite : image binaire.">

*Binarisation d'une image de grain de pollen. a gauche : image originale. A droite : image binaire. Par Ханжина Наталья Евгеньевна — Travail personnel, CC BY-SA 4.0, https://commons.wikimedia.org/w/index.php?curid=45015281*

## Opération morphologique

📖 [OpenCV - Opération morphologique](https://docs.opencv.org/4.13.0/d9/d61/tutorial_py_morphological_ops.html)

<img class="img-no-border" src="../DilationErosion.png" alt="Une forme (en bleu), sa dilatation morphologique (en vert), et son érosion morphologique (en jaune) par un élément structurant en forme de diamant.">

*Une forme (en bleu), sa dilatation morphologique (en vert), et son érosion morphologique (en jaune) par un élément structurant en forme de diamant. Par Renato Keshet — created by the user, Domaine public, https://commons.wikimedia.org/w/index.php?curid=4413072*

<img class="img-no-border" src="../Illustration_morpho.png" alt="Image originale (en noir : l'objet ; en blanc : le fond).">

*Image originale (en noir : l'objet ; en blanc : le fond). Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600427*

<img class="img-no-border" src="../Illustration_dilatation.png" alt="Dilatation par un carré 3x3 : les pixels noirs et gris font partie de l'ensemble résultant.">

*Dilatation par un carré 3x3 : les pixels noirs et gris font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600447*

<img class="img-no-border" src="../Illustration_erosion.png" alt="Érosion par un carré 3x3 : seuls les pixels noirs font partie de l'ensemble résultant.">

*Érosion par un carré 3x3 : seuls les pixels noirs font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600436*





<img class="img-no-border" src="../Illustration_fermeture.png" alt="Fermeture par un carré 3×3 : les pixels noirs et gris font partie de l'ensemble résultant.">

*Fermeture par un carré 3×3 : les pixels noirs et gris font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600457*

<img class="img-no-border" src="../Illustration_ouverture.png" alt="Ouverture par un carré 3×3 : seuls les pixels noirs font partie de l'ensemble résultant">

*Ouverture par un carré 3×3 : seuls les pixels noirs font partie de l'ensemble résultant. Par Etienne Decenciere — Travail personnel, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=4600455*






## Filtres

### Détection des bords

📖 [OpenCV - Gradients](https://docs.opencv.org/4.13.0/d5/d0f/tutorial_py_gradients.html)

<img class="img-no-border" src="../Intensity_image_with_gradient_images.png" alt="On the left, an intensity image of a cat. In the center, a gradient image in the x direction measuring horizontal change in intensity. On the right, a gradient image in the y direction measuring vertical change in intensity. Gray pixels have a small gradient; black or white pixels have a large gradient.">

*On the left, an intensity image of a cat. In the center, a gradient image in the x direction measuring horizontal change in intensity. On the right, a gradient image in the y direction measuring vertical change in intensity. Gray pixels have a small gradient; black or white pixels have a large gradient. By Njw000 - Own work, Public Domain, https://commons.wikimedia.org/w/index.php?curid=10588443*




📖 [OpenCV - Canny](https://docs.opencv.org/4.13.0/da/d22/tutorial_py_canny.html)

## Détection des lignes

📖 [OpenCV - Transformée de Hough](https://docs.opencv.org/4.13.0/d6/d10/tutorial_py_houghlines.html)