---
title: 🖼️ Unreal Engine Renovation for Nation
date: 2021-11-15T14:47:52+01:00
description: Découvrez comment HOK, une entreprise d'architecture et d'ingénierie, aide à préserver une icône nationale, le "Canada's Parliament Hill".
image: images/unreal/banner.jpg
categories:
- XR / VR
tags: 
- ArchViz
- Unreal Engine
- Photogrammétrie
- Environnements
---

Unreal Engine (UE) est un moteur de rendu utilisé principalement dans le domaine des jeux-vidéos *(Fortnite, Sea of Thieves, Batman: Arkham, ...)*.

Depuis quelques années, UE se diversifie, et s'attaque notamment au marché de la visualisation architecturale, ou *ArchViz* pour les intimes. 

Plongeons donc ensemble dans un article retraçant leur collaboration avec [HOK](https://www.hok.com/), une entreprise américaine active dans l'architecture et l'ingénierie, pour un projet de conservation historique.

## Un héritage virtuel

Au centre d'Ottawa se trouve l'Édifice du Centre *(Centre Block)*, bâtiment habritant le Sénat canadien, la Chambre des communes du Canada ainsi que divers bureaux de parlementaires. Ce bâtiment construit en 1916 est depuis 1987 classé comme lieu historique national.

Afin de conserver cette pièce de l'histoire canadienne, tout en continuant à l'utiliser pour les activités politiques quotidiennes, un projet de rénovation a été lancé afin de préserver cet héritage pour les générations futures.

Vu l'ampleur du projet, qui devrait se dérouler sur une dizaine d'années, HOK ont pris la décision de porter la planification à l'échelon supérieur.

En tirant parti des outils d'Unreal Engine et [Twinmotion](https://www.twinmotion.com/en-US) *(un outil d'ArchViz développé par UE)*, HOK est en train de développer une version réaliste virtuelle du bâtiment, visitable en réalité virtuelle.

En plus d'être une expérience interactive impressionnante au niveau technologique, ces visites permettent de voir en temps réel les résultats des différents travaux à venir.

## Comment ça marche ?

Sans entrer dans les détails techniques du développement, HOK dévoile leur workflow pour la mise en place de ce projet.

La création des maquettes commence par un joyeux mélange de données CAD (Computer-assisted design), scans à grandes et petites échelles, pour ensuite être reconstruit en 3D grâce à l'outil de photogrammétrie [RealityCapture](https://www.epicgames.com/site/fr/news/capturing-reality-is-now-part-of-epic-games), créé par UE.

La quantité de scans est simplement inhumaine : HOK rapporte avoir 100 TB de scans (sous la forme de nuage de points), et 70 TB de *meshes* (objets 3D texturés, et prêts à être utilisés dans UE). En effet, le bâtiment n'est pas le seul élément à modéliser. Toutes les pièces, tous les couloirs, tous les objets amovibles doivent passer au scan, pour pouvoir créer un résultat au plus proche de la réalité.

![Nuage de points](/images/unreal/dotscloud.jpg)

Les modèles sont ensuite adaptée une échelle 1:1, et optimisé pour le rendu VR à travers le programme [Houdini](https://www.sidefx.com/).

Finalement, tous ses éléments sont envoyés vers Unreal Engine pour créer les expériences VR.

## Design en temps réel

Dès le début, il était important pour HOK d'avoir une pipeline de production optimisée, afin de pouvoir montrer en temps réel les modifications planifiées. 

> “The greatest benefit in deploying real-time solutions is that they are real time!” - *Mark Cichy, CTO de HOK*

![Nuage de points](/images/unreal/room.jpg)

Ce genre de processus n'est pas pour "faire joli", mais permet de convaincre les investisseurs, d'obtenir des retours éclairées de tous les partis impliqués dans le projet, et surtout d'économiser des coûts de rénovation inutiles.

Finalement, le jumeau digital du Centre Block ne sera pas mis à la corbeille à la fin des rénovations, mais sera accessible et intégré au patrimoine culturel canadien.

## Conclusion

Cet article apportait de nombreuses informations, que j'ai classées en 3 catégories :

### 1. Les outils utilisés

Dans cet article, la transparence de HOK et UE m'a impressioné. En effet, il est parfois compliqué d'avoir un aperçu de la façon de travailler de ces entreprises à la pointe de la technologie.

Il est clair que pour UE, la majorité des *softwares* utilisés étaient leurs propres produits, mais ils ne manquaient pas de mentionner les programmes externes utilisés dans des tâches pour lesquels leurs programmes ne sont pas utilisables.

Du côté *hardware*, HOK mentionne également les différents types d'appareils utilisés pour leurs scans : caméras, drones, scanners terrestres, scanners portatifs *(pour les plus petits objets)*, ...

### 2. Le workflow

Finalement, je trouve la façon dont le processus de réalisation est expliqué très intéressante, car cela permet d'avoir un aperçu du début à la fin du projet. Cela permet aussi de se rendre compte de l'ampleur de la planification d'un tel projet.

### 3. Un exemple d'application de la VR

Il est clair qu'aujourd'hui, VR et architecture ne sont pas encore des mots associés régulièrement. Je pense qu'en effet, la réalité virtuelle peut avoir un immense impact sur les domaines de la construction et de la conservation, et c'est des pistes que je souhaite approfondir, notamment dans un contexte helvétique.

## Sources

Images : https://www.unrealengine.com/en-US/spotlights/renovation-for-the-nation-how-hok-is-helping-preserve-a-national-icon-on-canada-s-parliament-hill

