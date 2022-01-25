# Site

Disponible à cette adresse : [GitHub Page](https://mikael-ruffieux.github.io/labveiltech/)

## Bugs connus

[25.01.2022]

Il était demandé initialement de déployer notre site sur une **GitHub Page**. Malheureusement, à cause d'un problème que je n'ai pas réussi à identifier, le code publié ne prend pas en compte certains éléments, comme par exemple l'affichage des articles sur la page d'accueil.

Pour palier à ce problème, j'ai donc décidé de le publier sur mon propre hébergement, sous un sous-domaine : [labveiltech.redoxdigital.ch](https://labveiltech.redoxdigital.ch/).

[26.01.2022]

<ins>Mise à jour</ins> : j'ai pu finalement régler le problème. En effet, en local, pour générer mes pages statiques, j'utilisais la commande `hugo -D`, versus la commande `hugo`, ce qui générait toutes les pages, qu'importe leur statut. Il s'avérait que mes articles avaient tous le paramètre `draft: true`, ce qui empêchait la génération des articles qui avaient encore le statut de brouillon.

## Commandes

- Lancer le serveur : `hugo server -D`
- Nouvel article : `hugo new posts/my-first-post.md`
- Construire les pages statiques : `hugo`

## Taxonomie

### Catégories
- XR / VR
- Communication digitale
- 3D Design

### Tags
- VR
- AR
- Oculus
- Gaming
- ArchViz
- Tutoriel
- Unreal Engine
- Unity
- Blender
- Quixel Megascans
- webVR
- Photogrammétrie
- Texturing
- Environnements
- Suisse
- Musées
- Entreprises
