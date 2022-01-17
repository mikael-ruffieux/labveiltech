---
title: "VR Workflow : par où commencer ?"
date: 2022-01-17T10:31:19+01:00
description: "Il existe mille et une façons de créer une expérience VR, en utilisant mille et un outils pour créer une expérience VR. Parmis cette jungle d'informations et de technologies, par où commencer ?"
image: images/vr-workflow/workflow.png
draft: true
categories:
- XR / VR
tags: 
- Unreal Engine
- Unity
- Blender
- VR
- Oculus
---

Avec toutes ces recherches sur le sujet de la VR, de la XR, et de son utilisation sur le marché actuel, j'avais l'impression que toutes les routes menaient à Rome. Il existe mille et une façons de créer une expérience VR, en utilisant mille et un outils, payant ou non, pour arriver à la fin au Graal que je cherche à créer : une expérience VR.

La question que je me posais était la suivante : **à quoi ressemble le workflow d'un développeur VR** ? Par où commencer dans cette jungle d'informations ? 

Je suis alors tombé sur la vidéo du développeur VR Justin P. Barnett : https://www.youtube.com/watch?v=oqXBY51KP5A

Ce dernier présentait les différentes étapes du parcours d'un développeur VR, quelles questions devaient se poser ce dernier, et quels outils étaient à disposition d'un développeur en herbe.

### Avant de se lancer : essayer !

Son premier conseil était bien entendu de tester la VR avant de se lancer. En effet, les expériences de réalité virtuelle demandent une certaine aisance dans un environnement 3D. Justin déconseillait de se lancer comme développeur VR si on était particulièrement sensible à la cinétose (*motion sickness* en anglais).

J'avais eu l'occasion de tester la réalité virtuelle grâce à la HEIG-VD, en y empruntant un Oculus Quest 1.

### Les casques de réalité virtuelle

Concernant le *hardware*, le matériel à avoir pour commencer à développer en VR, Justin présentait une liste d'options, du casque meilleur marché au plus onéreux, avec pour chacun des avantages et inconvénients.

#### L'option bon marché

La première option, la moins chère, était celle du Google Cardboard (~12$), une option qui permet d'utiliser son smartphone comme support, avec des lentilles qui permettent de simuler cette vision stéréo. D'autres casques, comme le Google Daydream (79$), ou l'Oculus Gear VR (99$), permettent d'attendre le même résultat, avec un équipement un peu plus robuste qu'une monture en carton.

Avantages :
+ Prix abordable
+ Tout le monde a un smartphone
+ Facile à mettre en place

Désavantages :
- Matériel peu performant
- On sacrifie le confort pour des expériences VR plus longues

#### L'option médiane

Si on veut se lancer un peu plus sérieusement dans la VR, que ce soit du côté consommateur ou développeur, il recommandait l'Oculus Quest 2 (399$), qui est un casque indépendant, et qui n'a donc pas besoin d'être connecté à un ordinateur pour faire le rendu VR.

Il s'agit d'ailleurs du casque que je possède.

Avantages :
+ Haute qualité d'image
+ Portabilité
+ Compatibilité avec les dernières technologies VR
+ Rapport qualité-prix excellent
+ Peut être connecté à un ordinateur par câble ou via WiFi pour des expériences plus conséquentes

Désavantages :
- Peut être un gros investissement "juste pour essayer"
- Manque de puissance pour les expériences VR lourdes

#### L'option premium

Comme options haut de gamme, Justin mentionnait l'Oculus Rift S (799$), ou le HTC Vive (899$). Mais vu que sa vidéo s'adressait plutôt aux futurs développeurs VR, il ne s'est pas trop attardé sur ces casques.

Avantages :
+ Excellente qualité visuelle
+ Très bon tracking
+ Connexion directe à l'ordinateur (très utile pour le développement)

Désavantages :
- Onéreux
- Demande un ordinateur performant pour les rendus
- N'est pas transportable

### Quels programmes utiliser ?

Comme j'avais pu le remarquer au travers de mes recherches, les 2 mastodontes du marché des moteurs de jeu étaient [Unity](https://unity.com/fr) et [Unreal Engine](https://www.unrealengine.com).

#### Unreal Engine

Unreal Engine (UE) est principalement utilisé pour les jeux photoréalistes, qui demande beaucoup de ressources pour leur rendu, et/ou pour les jeux AAA, soit les jeux grand public.

Pour le développement, UE propose un environnement en C++, ou en utilisant un système de *Nodes*, qui s'apparentent à un développement en blocs.

#### Unity

Unity s'adresse plutôt aux studios indépendants, et utilise C# comme langage de programmation.

Initialement, j'avais porté mon choix sur Unreal Engine, car j'avais déjà eu l'occasion de l'utiliser pour des projets "bac à sable", et la programmation en blocs m'évitait de devoir apprendre un nouveau langage.

Mais après avoir discuté avec [Christophe Merkle](https://christophemerkle.com/), alumni de Comem+, et VR Specialist indépendant, il me recommandait plutôt de choisir Unity. Étant donné que je connaissais déjà Java, la transition à C# ne demanderait que peu d'effort, et Unity était plus adapté, notamment au niveau de l'optimisation pour des petits projets. Il mentionnait d'ailleurs que le système de *Nodes* de UE était pratique pour créer rapidement des algorithmes simples, mais devenait vite limitant pour des interactions plus complexes.

### Quelles compétences sont à développer ?

À ce stade-là, j'étais plutôt confiant, car j'avais déjà pu répondre aux différents critères mentionnés : j'avais déjà essayé la réalité virtuelle, je possédais un casque, et j'avais déjà pu m'essayer à Unreal Engine.

Mais c'est là que les choses se corsent.

Avant de se lancer dans le développement VR, Justin P. Barnett recommandait de s'essayer au développement de jeu en générale, notamment au travers des jeux à la première personne, qui ne sont qu'à un pas de la réalité virtuelle.

Autre point très important était la partie artisitique des projets de VR. En effet, développer un environnement 3D était une chose, mais encore fallait-il le remplir.

#### Game assets creation

Pour cela, il recommandait le programme gratuit [Blender](www.blender.org), ou les programmes payants [3DS Max](https://www.autodesk.ch/fr/products/3ds-max/overview) et [Maya](https://www.autodesk.fr/products/maya/overview).

#### Game assets libraries

Mais si la fibre artistique n'était pas notre fort, il listait aussi différentes bibliothèques d'objets 3D, gratuits ou non, avec notamment :

- [TurboSquid](https://www.turbosquid.com)
- [Free3D](https://free3d.com)
- [CGTrader](https://www.cgtrader.com)
- [Sketchfab](https://sketchfab.com)
- [Probuilder](https://unity.com/features/probuilder)

#### Sound design

Finalement, pour créer des expériences immersives, le son est un élément cruciale, et n'est pas à négliger.

Pour ce dernier, j'ai déjà une certaine expérience au design audio, grâce à mes compétences de réalisation vidéo.

### Conclusion

En fin de vidéo, Justin nous laissait sur le message suivant : regarder des vidéos et lire des articles sur le développent VR était une bonne chose, mais pour commencer à apprendre, et à s'améliorer, **il fallait commencer à développer ses propres projets** !

Après ce visionnage riche en apprentissage, j'ai donc créé une liste de ce que je savais déjà, de ce que je devais apprendre, et des différentes ressources mentionnées tout au long de la vidéo.

#### Ce que je possède déjà
- Un casque VR
- Un ordinateur performant pour les rendus
- Des compétences en design audio
- Des compétences en story-telling grâce à la vidéo

#### Ce qu'il me reste à apprendre
- La création 3D :
    - Modélisation
    - Textures
    - Optimisation pour les moteurs de rendu
- Le développement sur Unity :
    - C#
    - L'environnement de développement Unity
- Transposer mes compétences de sound-design et story-telling au monde de la VR

Cette liste m'a impressionné, et quelque peu découragé, je dois avouer... Mais j'ai pris mon courage à 2 mains, et j'ai commencer par ce qui me semblait être la première étape de mon apprentissage : l'utilisation de Blender et la modélisation d'objets en 3D.

Pour découvrir un des projets réalisés, rendez-vous sur l'article : [Fisherman's Shack](/labveiltech/posts/fishermans-shack/).



### Sources

Bannière : https://blog.trello.com/hs-fs/2018-04-24_WhatEvenIsAWorkflowAndWhyDoYouNeedIt_r01.png

