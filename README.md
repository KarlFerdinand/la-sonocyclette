# La SonoCyclette — site vitrine

Site one-page de **La SonoCyclette** : livraison de fête à vélo, sur place ou à emporter (Strasbourg).

En ligne : https://karlferdinand.github.io/la-sonocyclette/

## Contenu

- `index.html` — la page d'accueil (textes, styles et animations sont dans ce seul fichier)
- `tarifs.html` — la fiche tarifs (forfait, compléments, options, récapitulatif, conditions)
- `infos-pratiques.html` — la fiche pratique (dimensions du vélo, repérage du parcours, formats, à la charge de l'organisation)
- `assets/fiches.css` — les styles communs aux deux fiches
- `assets/la-sonocyclette-tarifs.pdf` et `assets/la-sonocyclette-infos-pratiques.pdf` — les fiches en PDF (A4, 3 pages chacune) à envoyer aux clients, téléchargeables depuis les pages. Elles ne se mettent pas à jour toutes seules : après un changement de tarif ou de texte, il faut les regénérer.

**Tarifs : à changer partout en même temps.** Le forfait (450 € HT) apparaît aussi sur l'accueil (bandeau, onglets Prestations, FAQ, bloc Devis et données Google en bas de `index.html`). En cas de changement de prix, chercher « 450 » dans les trois fichiers.
- `assets/` — photos, teaser vidéo, logo et icônes

## Modifier le site

1. Sur GitHub, ouvrir `index.html` puis cliquer sur le crayon (« Edit this file »).
2. Modifier le texte voulu (chercher le passage avec Ctrl+F).
3. Cliquer sur « Commit changes ». Le site se met à jour tout seul en 1 à 2 minutes.

Pour changer une photo : déposer la nouvelle image dans `assets/` avec **le même nom de fichier** que l'ancienne (« Add file » → « Upload files »).

**Photos : étalonnage et filigrane.** Les photos du site sont étalonnées de la même façon (balance des blancs, exposition, contraste, chaleur), recadrées au format exact de leur emplacement et portent un filigrane discret « LA SONOCYCLETTE » en bas de l'image (versions affichées et versions agrandies de la visionneuse ; pas sur le diaporama d'accueil). Une photo déposée telle quelle n'aura donc ni le même rendu ni le filigrane : le plus simple est de la transmettre pour qu'elle soit traitée avec la même chaîne.
Toutes les photos du site viennent de la photothèque de La SonoCyclette (aucune image tierce, aucun crédit à maintenir).

## Afficher le fil Instagram en direct (onglet « Actus Instagram »)

Le site peut afficher automatiquement les 6 dernières publications de @lasonocyclette grâce à [Behold](https://behold.so) (formule gratuite : 6 posts, mise à jour toutes les 24 h, 1 200 vues par mois — le fil ne se charge que quand un visiteur ouvre l'onglet).

1. Créer un compte gratuit sur behold.so et connecter le compte Instagram @lasonocyclette.
2. Créer un « Feed », choisir « Widget », puis copier son identifiant (le `feed-id`).
3. Sur GitHub, ouvrir `index.html`, chercher `INSTAGRAM_FEED_ID` et coller l'identifiant entre les guillemets :
   `var INSTAGRAM_FEED_ID = "votre-identifiant";`
4. « Commit changes » : le fil apparaît sur le site en 1 à 2 minutes.

Tant que l'identifiant est vide, l'onglet « Actus Instagram » reste masqué (le lien « Plus de photos sur Instagram » sous la galerie suffit). Il apparaît automatiquement dès que l'identifiant est renseigné.

## Référencement Google (à faire une fois le site en ligne)

Le site contient déjà : titre et description ciblés (« DJ & sono à vélo à Strasbourg »), données structurées (entreprise + FAQ), `sitemap.xml` et `robots.txt`.

1. **Google Search Console** : ajouter le site, puis envoyer `sitemap.xml` (Sitemaps → ajouter).
2. **Google Business Profile** : créer la fiche « La SonoCyclette » (catégorie « Disc-jockey » ou « Service d'animation d'événements »), zone desservie Strasbourg + Eurométropole, lien vers le site, photos. C'est le levier n° 1 pour apparaître dans les recherches locales et sur Google Maps.
3. **Avis** : après chaque prestation, envoyer le lien d'avis Google aux clients.
4. **Annuaires** : mêmes nom / téléphone / e-mail partout (Mariages.net, Pages Jaunes, annuaires événementiels locaux).
5. **Instagram** : mettre le lien du site dans la bio de @lasonocyclette.

Si le site passe un jour sur un nom de domaine propre (ex. lasonocyclette.fr), remplacer l'adresse `karlferdinand.github.io/la-sonocyclette` dans `index.html`, `sitemap.xml` et `robots.txt`.

## Recevoir les demandes de devis directement par e-mail

Par défaut, le formulaire ouvre la messagerie du visiteur. Pour recevoir les demandes directement :
1. Sur [web3forms.com](https://web3forms.com), saisir ivan.vollet@gmail.com pour obtenir une clé gratuite.
2. Dans `index.html`, chercher `FORM_ACCESS_KEY` et coller la clé entre les guillemets.

## Mentions légales

La page `mentions-legales.html` indique Artenréel Spectacle comme structure éditrice (siège, RCS, SIRET, TVA) et Ivan Vollet comme directeur de la publication.

## Statistiques de visite (GoatCounter)

1. Créer un compte gratuit sur [goatcounter.com](https://www.goatcounter.com/signup) avec le code `lasonocyclette`.
2. Dans `index.html`, chercher `GOATCOUNTER_CODE` et écrire `lasonocyclette` entre les guillemets.
Sont comptés : pages vues, demandes de devis, clics sur le téléphone, l'e-mail et Instagram. Aucun cookie.

## Contact

Ivan Vollet — ivan.vollet@gmail.com — Instagram [@lasonocyclette](https://www.instagram.com/lasonocyclette/)

Projet soutenu par la DRAC Grand Est et Artenréel #1.
