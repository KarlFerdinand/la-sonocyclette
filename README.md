# La SonoCyclette — site vitrine

Site one-page de **La SonoCyclette** : livraison de fête à vélo, sur place ou à emporter (Strasbourg).

En ligne : https://karlferdinand.github.io/la-sonocyclette/

## Contenu

- `index.html` — toute la page (textes, styles et animations sont dans ce seul fichier)
- `assets/` — photos, teaser vidéo, logo et icônes

## Modifier le site

1. Sur GitHub, ouvrir `index.html` puis cliquer sur le crayon (« Edit this file »).
2. Modifier le texte voulu (chercher le passage avec Ctrl+F).
3. Cliquer sur « Commit changes ». Le site se met à jour tout seul en 1 à 2 minutes.

Pour changer une photo : déposer la nouvelle image dans `assets/` avec **le même nom de fichier** que l'ancienne (« Add file » → « Upload files »).

## Afficher le fil Instagram en direct (onglet « Actus Instagram »)

Le site peut afficher automatiquement les 6 dernières publications de @lasonocyclette grâce à [Behold](https://behold.so) (formule gratuite : 6 posts, mise à jour toutes les 24 h, 1 200 vues par mois — le fil ne se charge que quand un visiteur ouvre l'onglet).

1. Créer un compte gratuit sur behold.so et connecter le compte Instagram @lasonocyclette.
2. Créer un « Feed », choisir « Widget », puis copier son identifiant (le `feed-id`).
3. Sur GitHub, ouvrir `index.html`, chercher `INSTAGRAM_FEED_ID` et coller l'identifiant entre les guillemets :
   `var INSTAGRAM_FEED_ID = "votre-identifiant";`
4. « Commit changes » : le fil apparaît sur le site en 1 à 2 minutes.

Tant que l'identifiant est vide, l'onglet affiche la carte du profil et un lien vers Instagram.

## Contact

Ivan Vollet — ivan.vollet@gmail.com — Instagram [@lasonocyclette](https://www.instagram.com/lasonocyclette/)

Projet soutenu par la DRAC Grand Est et Artenréel #1.
