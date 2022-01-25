---
title: "🐟 Fishermans Shack : mon apprentissage de Blender"
date: 2022-01-17T12:15:50+01:00
description: "Premier gros projet de modélisation 3D, j'ai suivi une série de vidéos montrant comment utiliser les outils de Blender."
image: images/fisherman/preview.jpeg
draft: true
categories:
- 3D Design
tags: 
- Tutoriel
- Blender
- Texturing
- Environnements
---

Pour cette partie plus pratique, comme mentionné dans mon article sur [le workflow à suivre pour du développement VR](/posts/vr-workflow), je mentionne à la fin une expérimentation.

Après avoir suivi quelques tutoriels sur l'utilisation de tel ou tel outils sur Blender, je voulais suivre un tutoriel plus complet, et créer une scène de A à Z. Je suis alors tombé sur la série de vidéos du YouTuber [Grant Abbitt](https://www.youtube.com/channel/UCZFUrFoqvqlN8seaAeEwjlw). C'est sa série de 12 vidéos, pour un total de 165 min (2h45), qui m'a finalement attiré.

## Le *modeling*

Pour commencer, il fallait construire notre petite baraque. Pour ceci, j'ai créé différents types de planches et de poutres, qu'il me faudrait ensuite assembler pour construire ma cabane. J'ai créé 4-5 planches uniques, 2 types de poutres, et je les ai ensuite dupliquées, et légèrement modifiées, pour créer mon plancher, mes murs et les différents supports de ma cabane.

![Planches initiales](/images/fisherman/planks.png)

Une fois ma cabane construite, je n'ai pas résisté à texturer grossièrement les planches et différents éléments de cette dernière : 

![Cabane](/images/fisherman/shack1.png)

### Les accessoires

La création des accessoires a été ma partie préférée. En effet, je trouve incroyable comme à partir des formes de base (cube, cylindre, etc.), et grâce à quelques modifications, on arrive très rapidement à des objets simples, mais reconnaissables. 

Si je me suis fortement inspiré des objets présents dans la scène de Grant Abbitt, je n'ai pas suivi le tutoriel pour cette partie, j'ai préféré découvrir par moi-même.

![Accessoires](/images/fisherman/accessoires.png)

## Le *sculpting*

Pour l'environnement de cette cabane, toujours en suivant le tutoriel, j'ai créé différents caillous et rochers, que j'ai disposé dans ma scène. Comme il s'agit ici d'éléments organiques, j'ai donc utiliser des outils de *sculpting* pour créer des formes irrégulières, et qui gardait ce style *Low Poly*. 

Pour les algues qui recouvrent le fond marin, c'était relativement simple : j'ai créé une première algue, que j'ai ensuite dupliquée et distribuée à l'aide d'une *weight map* sur mon sable. Le modificateur utilisé permettait de rendre le positionnement, la rotation et l'échelle des algues copiées aléatoires, ce qui permettait un peuplement quasi organique.

La *weight map* permet de contrôler la distribution des algues sur la surface du sable. Les zones rouges représentent une haute densité de peuplement, tandis que les zones bleues représente une densité basse, voire nulle.

![Weigth Map & algue](/images/fisherman/wmap+algue.png)

Pour les poissons qui peuplaient mes eaux, Grant Abbitt proposait un tutoriel pour les créer, mais je trouvais les poissons trop simplistes, et leur design ne me plaisait pas. J'ai donc été chercher une sélection de modèles gratuits sur [Sketchfab](https://sketchfab.com/feed), pour donner un peu plus de qualité et de diversité à ma faune maritime.

## Les animations

À ce stade, ma scène était terminée, mais statique :

![Shack 2](/images/fisherman/shack2.png)

La prochaine et dernière étape était d'animer 3 éléments : la caméra, mes poissons, et le drapeau.

Du plus simple au plus compliqué, j'ai commencé par animer ma caméra. En effet, il suffisait de définir sa trajectoire en cercle, et de définir un point sur lequel l'objectif devait se braquer (ici, le centre de mon modèle), et l'affaire était jouée !

### Les *armatures*

Pour le drapeau, j'avais initialement utilisé une méthode découverte dans un autre tutoriel, une technique qui consistait à utiliser l'outil de **simulation de tissu** intégré à Blender, puis d'ajouter un souffle d'une certaine force dans la direction souhaitée. Si cette technique fonctionnait tout à fait, Grant Abbitt proposait une autre approche : celle de créer un "squelette" pour mon drapeau, et d'animer directement ce dernier, afin de pouvoir facilement boucler l'animation.

Comme je n'avais encore jamais utilisé d'armature, j'ai sauté sur l'occasion pour en apprendre plus.

Sans entrer dans les détails de la procédure, j'ai pu comprendre le fonctionnement de ces squelettes, et la manière d'animer chaque os et articulations individuellement, ainsi que la manière d'attribuer une section de notre *mesh* à chaque os.

![Armature du drapeau](/images/fisherman/drapeau.png)

Pour les poissons, la procédure était simplement une combinaison des deux techniques apprises au-préalable : d'abord, animer les poissons individuellement, en utilisant comme référence une image décomposant le mouvement de nage d'un poisson :

![Décomposition de la nage d'un poisson](/images/fisherman/swim.gif)

Finalement, il me suffisait de définir la trajectoire que devait suivre le poisson. De manière similaire à mon mouvement de caméra, j'ai opté pour un mouvement en cercle :

![L'animation terminée](/images/fisherman/swiming-fish.gif)

## Conclusion

Après bien quelques heures de travail, voici le résultat final :

{{< iframe "https://sketchfab.com/models/a0809170db94473b865929c411f2afae/embed" >}}

Pour une raison qui m'échappe, l'eau est affichée opaque sur [SketchFab](https://sketchfab.com). Il est clair que tout n'est pas parfait, mais je suis content d'être arrivé à la fin de cette série de tutoriels, qui m'a beaucoup appris, et qui m'a permis de découvrir **un grand nombre d'outils** dans Blender.

Il est clair que l'utilisation de ce programme doit être un **apprentissage continu**, et s'il est "facile" de copier le travail d'un autre pour apprendre, il est plus difficile de créer ses propres objets 3D, mais ça sera pour la prochaine étape de mon apprentissage.

Un des éléments que j'ai trouvé le plus difficile, c'était la **création de textures** pour mes objets. S'il est facile d'appliquer une couleur de base à un objet, et de rapidement définir sa réflection et sa rugosité, j'ai trouvé assez compliqué de créer des bonnes textures, notamment la texture de l'eau ... 

Mais je pense qu'un des prochaines tutoriels que je suivrai sera sur [Substance Painter](https://www.substance3d.com/), l'outil de *texturing* 3D d'Adobe et qui nous est mis à disposition à travers la licence étudiante.

## Sources

La série de vidéos : https://www.youtube.com/watch?v=Jmir2bDpZA4&list=PLn3ukorJv4vsIOjZoMToZusH2uOyjCu6G
