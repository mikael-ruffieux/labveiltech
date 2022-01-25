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

![Accessoires](/images/fisherman/_planks_.png)

## Le *sculpting*

Pour l'environnement de cette cabane, toujours en suivant le tutoriel, j'ai créé différents caillous et rochers, que j'ai disposé dans ma scène. Comme il s'agit ici d'éléments organiques, j'ai donc utiliser des outils de *sculpting* pour créer des formes irrégulières, et qui gardait ce style *Low Poly*. 

Pour les algues qui recouvrent le fond marin, c'était relativement simple : j'ai créé une première algue, que j'ai ensuite dupliquée et distribuée à l'aide d'une *weight map* sur mon sable. Le modificateur utilisé permettait de rendre le positionnement, la rotation et l'échelle des algues copiées aléatoires, ce qui permettait un peuplement quasi organique.

![Algue](/images/fisherman/algue.png)

La *weight map* permet de contrôler la distribution des algues sur la surface du sable. Les zones rouges représentent une haute densité de peuplement, tandis que les zones bleues représente une densité basse, voire nulle.

![Weigth Map](/images/fisherman/weigth-map.png)

Pour les poissons qui peuplaient mes eaux, Grant Abbitt proposait un tutoriel pour les créer, mais je trouvais les poissons trop simplistes, et leur design ne me plaisait pas. J'ai donc été cherché une sélection de modèles gratuits sur [Sketchfab](https://sketchfab.com/feed), pour donner un peu plus de qualité et de diversité dans ma faune maritime.

## Les animations

À ce stade, ma scène était terminée, mais statique :

![Shack 2](/images/fisherman/shack2.png)

La prochaine et dernière étape était d'animer 3 éléments : la caméra, mes poissons, et le drapeau.

Du plus simple au plus compliqué, j'ai commencé par animer ma caméra. En effet, il suffisait de définir sa trajectoire en cercle, et de définir un point sur lequel l'objectif devait se braquer (ici, le centre de mon modèle), et l'affaire était jouée !

### Les *armatures*

Pour le drapeau, j'avais initialement utilisé une méthode découverte dans un autre tutoriel, une technique qui consistait à utiliser l'outil de simulation de tissu intégré à Blender, puis d'ajouter un souffle d'une certaine force dans la direction souhaitée. Si cette technique fonctionnait tout à fait, Grant Abbitt proposait une autre approche : celle de créer un "squelette" pour mon drapeau, et d'animer directement ce dernier, afin de pouvoir facilement boucler l'animation.

Comme je n'avais encore jamais utilisé d'armature, j'ai sauté sur l'occasion pour en apprendre plus.

Sans entrer dans les détails de la procédure, j'ai pu comprendre le fonctionnement de ces squelettes, et la manière d'animer chaque os et articulations individuellement, ainsi que la manière d'attribuer une section de notre *mesh* à chaque os.

![Armature du drapeau](/images/fisherman/drapeau.png)

Pour les poissons, la procédure était simplement une combinaison des deux techniques apprises au-préalable : d'abord, animer les poissons individuellement, en utilisant comme référence une image décomposant le mouvement de nage d'un poisson :

![Décomposition de la nage d'un poisson](/images/fisherman/swim.gif)

Finalement, il me suffisait de définir la trajectoire que devait suivre le poisson. De manière similaire à mon mouvement de caméra, j'ai opté pour un mouvement en cercle :

![L'animation terminée](/images/fisherman/swiming-fish.gif)

## Conclusion

<div class="sketchfab-embed-wrapper"> <iframe title="Fisherman's Shack" frameborder="0" allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" allow="autoplay; fullscreen; xr-spatial-tracking" xr-spatial-tracking execution-while-out-of-viewport execution-while-not-rendered web-share src="https://sketchfab.com/models/a0809170db94473b865929c411f2afae/embed"> </iframe> <p style="font-size: 13px; font-weight: normal; margin: 5px; color: #4A4A4A;"> <a href="https://sketchfab.com/3d-models/fishermans-shack-a0809170db94473b865929c411f2afae?utm_medium=embed&utm_campaign=share-popup&utm_content=a0809170db94473b865929c411f2afae" target="_blank" style="font-weight: bold; color: #1CAAD9;"> Fisherman's Shack </a> by <a href="https://sketchfab.com/rdX-TheArrow?utm_medium=embed&utm_campaign=share-popup&utm_content=a0809170db94473b865929c411f2afae" target="_blank" style="font-weight: bold; color: #1CAAD9;"> rdX-TheArrow </a> on <a href="https://sketchfab.com?utm_medium=embed&utm_campaign=share-popup&utm_content=a0809170db94473b865929c411f2afae" target="_blank" style="font-weight: bold; color: #1CAAD9;">Sketchfab</a></p></div>

## Sources

La série de vidéos : https://www.youtube.com/watch?v=Jmir2bDpZA4&list=PLn3ukorJv4vsIOjZoMToZusH2uOyjCu6G
