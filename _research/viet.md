---
title: "Débruitage et super-résolution pour les images bio-médicales"
excerpt: ""
project_date: 2014-2018
project_end: 2018
# hidden: true
header:
  teaser: /assets/Research/viet1.png
tags:
  - Matlab
---

Ce projet concerne la restauration d'images biomédicales (Scanner CT et IRM) en collaboration 
avec Françoise Dibos (PU LAGA/P13), Marie
Luong (MCF L2TI/P13), Jean-Marie Rocchisani (MCF-PH, radiologue Hôpital Avicennes/P13).
J’ai co-encadré avec M. Luong le stage de M2 de Dai Viet Tran en 2014, qui a été poursuivi en
thèse de doctorat sous la direction de F. Dibos (co-directeurs S. Li-Thiao-Té et M. Luong). Les
travaux ont porté sur la restauration d’images (débruitage et super-résolution), et ma contribution a
porté sur l’étude de la structure de l’espace des images au travers d’une représentation par patchs.

Quatre publications en conférence internationale avec actes ont été produites : 
- [12] montre que l’on peut améliorer la performance d’un algorithme de restauration d’images en
appliquant une transformation de Anscombe, c’est-à-dire en transformant le bruit poissonien en
un bruit gaussien afin d’utiliser une méthode adaptée au bruit gaussien.
- [13] montre que l’on peut améliorer la performance d’un algorithme de restauration d’images en
choisissant une topologie de type « transport optimal » (Earth Mover’s Distance) dans l’espace
des images, qui est plus adaptée à l’invariance par translation/rotation que la distance euclidienne.
- [15] montre que l’on peut améliorer la performance d’un algorithme de restauration d’images en
modélisant la distribution a priori dans un sous-espace vectoriel de faible dimension, au lieu
d’utiliser un a priori arbitraire parcimonieux. On fournit de plus une méthode efficace pour la
résolution du problème de minimisation dans ce cas.
- [16] montre que l’espace des images a une structure « isolée », car lorsque l’on utilise un modèle
de mélange comme a priori, la plus grande composante contient l’essentiel de l’information. Les
expériences menées montrent également que le nombre de composantes a peu d’incidence, mais
que le choix de la paramétrisation (le dictionnaire de patch) est prépondérant.