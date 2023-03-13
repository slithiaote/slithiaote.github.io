---
title: Logiciel Lepton et Recherche Reproductible
project_date: "2012-présent"
project_end: 2040
excerpt: ""
header:
  teaser: /assets/Research/lepton_teaser.png
tags:
  - Ocaml
  - Lepton
toc: true
---

## Recherche reproductible

La **recherche reproductible** est une démarche qui vise à rendre les travaux de recherche (articles, codes sources, etc.) 
facilement réutilisables par les lecteurs.

Elle s'intéresse à différents aspects du processus de présentation des résultats scientifiques :
- disponibilité des données
- ouverture des codes sources
- reproductibilité des résultats
- publication des travaux 

Je travaille plus particulièrement sur la reproductibilité et la réutilisation des résultats :
- reproduire les scripts d'analyse et les figures
- comprendre le code source en relation avec la méthode proposée
- organiser les différents éléments d'un travail pour faciliter sa réutilisation. 

Ce travail a conduit à 2 publications en conférence internationale, une publication dans un journal, une invitation 
dans 3 colloques nationaux (2 en France et 1 aux États-Unis) et l’organisation d’un workshop (au sein de la conférence SMAI2013).

## Logiciel Lepton

Depuis 2011, je développe le logiciel Lepton pour la recherche reproductible. 
C'est un logiciel open source disponible sur [GitHub](https://github.com/slithiaote/lepton)

Lepton utilise une approche de type « literate programming », dans la lignée des travaux de D. Knuth et des logiciels WEB et noweb. 
Par rapport aux autres logiciels de ce type, il est conçu pour la documentation de scripts d’analyse de données 
plutôt que pour la documentation du code source de librairies logicielles. 
En particulier, ses fonctionnalités permettent de faire travailler ensemble plusieurs logiciels ou 
langages de programmation (C, R, Python, Ocaml, Matlab, etc.) et de s’affranchir des règles syntaxiques pour la documentation.

Ainsi, le format de fichier texte retenu permet de garantir que les « documents exécutables » restent utilisables à très long terme, 
sans la nécessité de maintenir une infrastructure logicielle lourde.

## Intégration continue pour la recherche reproductible

L'intégration continue comme un moyen de garantir l’exécution correcte d'une analyse de données, dans un environnement contrôlé. 
Cette approche est étroitement reliée à la notion de "build system" et à la modularité des codes sources.

Dans le cadre de ces travaux, j’ai commencé à mettre en place un dépôt Gitlab sur la [plateforme PLMLab du CNRS](https://plmlab.math.cnrs.fr/), 
et à configurer le système d’intégration continue. J'étudie en ce moment [bazel](https://bazel.build/) pour la compilation incrémentale.

L’achat d’un serveur de calcul est envisagé pour 2021, afin de pouvoir traiter les données médicales dans un environnement sécurisé. 
Ces développements ont été présentés lors du séminaire de l’équipe MBI en 2020 et au séminaire du master de mathématiques de P8 en 2021.

## Comité national pour la Science Ouverte

Depuis juin 2021, je participe aux travaux du [Comité national pour la Science Ouverte](https://www.ouvrirlascience.fr/open-science/), dans le collège Publications. 

Le collège a produit un [guide pratique sur la stratégie de rétention des droits d’auteur](https://www.ouvrirlascience.fr/mettre-en-oeuvre-la-strategie-de-non-cession-des-droits-sur-les-publications-scientifiques/)
et nous travaillons sur un référentiel des travaux publiés sous forme de badges 
(ouverture des données, des codes sources, licences, type de relecture par les pairs, etc.)