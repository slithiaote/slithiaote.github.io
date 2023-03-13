---
title: Vidéos Endoscopiques de l'Intestin
# toc: true
excerpt: ""
project_date: 2018-présent
project_end: 2023
header:
  teaser: /assets/Research/colon.png
tags:
  - Python
  - OpenCV
---

## Maladies Inflammatoires Chroniques de l'Intestin (MICI)

Avec le service de gastro-entérologie de l’hôpital Bichat-Beaujon, je travaille sur l’analyse de vidéos de coloscopie 
pour le diagnostic des maladies inflammatoires chroniques de l’intestin (rectocolite hémorragie et maladie de Crohn) 
et la prédiction de la réponse au traitement. Dans cette application, les médecins évaluent la sévérité de la maladie 
suivant la présence d’inflammation, de saignements ou d’ulcères sur la paroi intestinale. Cependant, les recommandations 
actuelles conduisent à négliger le nombre et la répartition spatiale des lésions et à ne considérer que la lésion la plus 
grave observée, en raison de l’absence d’outil logiciel et de travaux scientifiques.

Nous avons recruté une étudiante, Safaa Al Ali, en stage de M2, puis en thèse de doctorat afin d’aborder à la fois les 
aspects traitement d’image (co-directeur S. Li-Thiao-Té) et les aspects modélisation par équations aux dérivées partielles (directeur H Zaag). 
Le financement a été apporté par le DIM MathInnov de la région Ile-de-France.

## Analyse des vidéos endoscopiques

Dans un premier temps, le travail a porté sur la définition de détecteurs des lésions élémentaires (saignements et ulcères), 
et leur positionnement dans le colon. Une première version de ces détecteurs est en cours de finalisation, et a donné 
lieu à une représentation schématique (cf ci-dessous) qui sera validée avec les médecins. Ce travail a été présenté sous 
la forme d’un poster lors de l’école de recherche « Mathematics for Signals, Images and Structured Data » début 2021. 
Un manuscrit a été soumis à la conférence CAIP 2021.

{% include figure image_path="/assets/Research/colon.png" alt="Colon" width="50%" 
   caption="Colon atteint de RCH (saignements en rouge, ulcères en vert)." %}

## Modélisation par une équation de réaction diffusion

À partir des lésions détectées (automatiquement ou annotées par le médecin), nous souhaitons décrire la répartition des lésions, 
et relier cette description à l’état du patient ou à sa réponse à certains types de médicaments.

Actuellement, nous travaillons sur la relation entre la répartition des lésions et le score UCEIS qui est fourni par 
les médecins et indique la sévérité de la maladie. Étant donné un ensemble de modèles, qui est ici l’ensemble des solutions d’une EDP,
on commence par classer chaque modèle en : répartition uniforme, sur-abondance en zone iléale ou sur-abondance en zone anale. 
On classe ensuite les observations de chaque patient suivant les paramètres du modèle. Les premiers résultats ont été présentés 
lors de la conférence « Mathematics of complex systems in biology and medecine » au CIRM en février 2020.

Nous travaillons également sur l’application d’un modèle de propagation de la maladie basé sur l’équation de Fisher-KPP 
(équation de réaction-diffusion). Ce modèle prédit l’apparition de fronts d’onde, et nous souhaitons calculer la vitesse 
de ces fronts à partir du coefficient de diffusion estimé pour chaque patient. Ci-dessous un exemple de simulation de la 
propagation de la maladie à partir du profil d’inflammation d’un patient à t=0. 

{% include figure image_path="/assets/Research/test-patient-23-New.png" alt="Patient23" width="50%" 
   caption="Modèle de Fisher-KPP appliqué au patient 23." %}