# Prompt pour recreer l'Atelier d'etiquettes de potions

Tu es un developpeur frontend senior. Cree une webapp statique locale, sans dependances ni build, pour creer et editer des stickers vintage de potions destines a un cosplay, un GN ou une vitrine fantastique.

## Objectif

Construire un editeur d'etiquettes de potions directement utilisable dans un navigateur via un simple fichier `index.html`, avec `styles.css` et `app.js`. L'utilisateur doit pouvoir composer des etiquettes imprimees en haute qualite, modifier leur contenu, importer des images, deplacer les blocs et exporter le resultat.

## Experience attendue

L'interface doit afficher :

- un panneau d'edition a gauche ;
- un grand apercu central de l'etiquette ;
- une planche imprimable avec plusieurs etiquettes ;
- un panneau a droite pour deplacer, aligner et selectionner des exemples.

L'app doit etre en francais et fonctionner hors ligne. Elle doit etre suffisamment simple pour etre ouverte depuis un dossier local, sans serveur.

## Fonctionnalites obligatoires

### Edition du contenu

Ajouter des champs pour modifier :

- le nom de la potion ;
- le sous-titre ;
- le texte fin ou la liste d'ingredients ;
- le nom de l'apothicaire ou fabricant ;
- le numero de lot ;
- le flacon, sous forme de champ texte libre ;
- la largeur globale en millimetres ;
- la hauteur globale en millimetres ;
- la taille du symbole ;
- l'opacite du fond importe.

### Formes

Les etiquettes doivent etre dessinees en SVG, pas seulement en HTML/CSS, afin que les contours suivent parfaitement la decoupe.

Prevoir au moins ces formes :

- rectangle vertical ;
- arche ;
- badge ;
- diamant ;
- blason ;
- ticket.

Chaque forme doit avoir :

- un contour externe ;
- un contour interne ;
- un contour interne pointille ou decoratif ;
- un fond papier texture.

### Export

Ajouter les exports suivants :

- PNG haute qualite ;
- SVG ;
- PDF via une page d'impression dediee ;
- JSON contenant l'etat courant et la planche.

Le PNG doit etre calcule en 300 dpi avec la formule :

```text
pixels = millimetres x 300 / 25,4
```

Le SVG et le PDF doivent utiliser les dimensions physiques choisies par l'utilisateur en millimetres.

### Images importees

Permettre :

- d'importer un PNG, JPG ou SVG pour remplacer le symbole central ;
- de glisser-deposer ce symbole ;
- d'importer un PNG, JPG ou SVG pour le fond de l'etiquette ;
- de glisser-deposer ce fond ;
- de regler l'opacite du fond.

Le fond importe doit rester decoupe dans la forme de l'etiquette avec un `clipPath`.

### Deplacement et alignement

Les blocs suivants doivent etre deplacables :

- apothicaire ;
- symbole ;
- nom ;
- sous-titre ;
- texte fin ;
- numero / flacon.

Proposer plusieurs moyens de deplacement :

- drag a la souris ou au tactile ;
- sliders X/Y ;
- boutons fleches ;
- fleches du clavier ;
- Shift + fleches pour deplacer plus vite.

Ajouter des options d'alignement :

- aligner a gauche ;
- centrer horizontalement ;
- aligner a droite ;
- aligner en haut ;
- centrer verticalement ;
- aligner en bas ;
- centrer completement ;
- reset de l'element selectionne.

### Exemples

Inclure au moins douze exemples d'etiquettes :

- Deadly Nightshade ;
- Mermaid Tears ;
- Love Potion ;
- Elixir of Life ;
- Phoenix Ashes ;
- Moon Dust ;
- Dragon's Breath ;
- Basilisk Venom ;
- Ghost Ink ;
- Royal Antidote ;
- Snail Slime ;
- Vampire Tonic.

Chaque exemple doit avoir sa forme, sa palette, son symbole, son texte et ses dimensions par defaut.

## Direction visuelle

Le style doit evoquer des etiquettes d'apothicaire anciennes :

- papier creme, beige, vert pale, rose poudre, bleu grise ;
- contours graves, doubles ou pointilles ;
- ornements simples ;
- typographies serif, script, poster et blackletter ;
- aspect imprime, artisanal, lisible ;
- pas de page marketing, l'editeur doit etre le premier ecran.

Eviter une palette trop uniforme. Utiliser des tons papier varies et des contrastes suffisamment forts pour l'impression.

## Contraintes techniques

- Utiliser seulement HTML, CSS et JavaScript vanilla.
- Ne pas utiliser de framework.
- Ne pas utiliser de build step.
- Garder les fichiers lisibles et faciles a modifier :
  - `index.html` pour la structure ;
  - `styles.css` pour l'interface ;
  - `app.js` pour les donnees, le rendu SVG, les exports et les interactions.
- Le rendu principal doit etre un SVG avec `viewBox`.
- Les exports doivent partir du meme SVG que l'aperçu pour eviter les differences visuelles.
- Le texte doit etre echappe avant insertion dans le SVG.
- Les images importees doivent etre lues en `data:` URL via `FileReader`.
- Le PDF peut etre genere en ouvrant une nouvelle fenetre HTML avec le SVG et `window.print()`.

## Livraison attendue

Produire les fichiers suivants :

- `index.html`
- `styles.css`
- `app.js`
- `README.md`

Le README doit expliquer :

- comment ouvrir l'app ;
- les fonctionnalites ;
- les exports ;
- la formule 300 dpi ;
- les exemples inclus.

Le resultat final doit permettre a un utilisateur non technique de creer, ajuster, exporter et imprimer des stickers de potions de qualite cosplay.
