# Atelier d’étiquettes de potions

Webapp locale pour créer et éditer des stickers de potions pour un cosplay.

## Utilisation

Ouvre `index.html` dans ton navigateur. L’app fonctionne sans installation et les principales polices décoratives sont incluses localement.

C’est également disponible [ici](https://maelremrem.github.io/PotionStickers/).

## Nouveautés

- Interface restructurée en trois étapes : composer, prévisualiser et ajuster.
- Panneaux fixes, groupes de réglages repliables et adaptation mobile améliorée.
- Sliders utilisables sur toute leur largeur, avec piste remplie et valeurs extrêmes visibles.
- Déplacement tactile et souris fiabilisé, avec mise à jour fluide de l’aperçu.
- 17 styles typographiques et 36 symboles alchimiques, célestes et décoratifs.
- Retours visuels lors de l’ajout, de la validation et de la réinitialisation.
- Navigation clavier et styles de focus plus accessibles.
- Historique annuler/rétablir avec raccourcis clavier et sauvegarde automatique du brouillon sur l’appareil.
- Taille, rotation et police personnalisables indépendamment pour chaque élément.
- Symbole agrandissable jusqu’à 200 % et taille de police réglable de 25 à 250 % pour chaque bloc texte.
- Boutons de réinitialisation séparés pour la position, l’échelle, la rotation, la taille typographique et la police de l’élément actif.
- Inspecteur universel : position, échelle, rotation et opacité pour tous les éléments ; graisse et espacement pour les textes ; épaisseur de trait pour les cadres et ornements.
- Décorations victoriennes, célestes, botaniques, alchimiques et runiques avec quantité, taille et couleur réglables.
- Générateur d’usure reproductible par seed : patine, taches, rayures, brûlures et auréoles, avec intensité réglable.
- Taches générées par bruit fractal de type Perlin et masques SVG : échelle, octaves, couverture, contraste, adoucissement et usure des bords réglables finement.
- Préréglages cohérents « Patine subtile », « Apothicaire authentique », « Cave humide » et « Reliquaire brûlé », plus couleur et mode de fusion personnalisables.
- Formats A4, A3 et A5, organisation automatique, marge de coupe et traits de coupe dans les planches PDF.
- Polices décoratives intégrées directement aux SVG et aux rendus PDF/PNG.
- Bibliothèque de modèles personnalisés avec duplication, favoris et import de projets JSON.

- Rendu SVG vectoriel : les contours externes et internes suivent la decoupe.
- Dimensions libres en millimetres pour la largeur et la hauteur. Les exports PNG sont calcules a 300 dpi.
- Exports unitaires : PNG HD, SVG et PDF via la fenetre d'impression du navigateur.
- Liste de designs valides via le bouton `Ajouter a la liste des exports` pour preparer plusieurs etiquettes avant export groupe.
- Export groupe depuis une modal : ZIP de PNG HD, ZIP de PDF HD, ou un seul PDF avec tous les designs cote a cote avec 2 mm de marge.
- Plus d'exemples : Deadly Nightshade, Mermaid Tears, Love Potion, Elixir of Life, Phoenix Ashes, Moon Dust, Dragon's Breath, Basilisk Venom, Ghost Ink, Royal Antidote, Snail Slime, Vampire Tonic.
- Plus de formes : rectangle, arche, badge, diamant, blason, ticket.
- Plus de polices de titre et de symboles.
- Le numéro et le flacon sont des champs texte libres.
- Le symbole central peut etre remplace par un PNG, JPG ou SVG depose.
- Le fond de l'etiquette peut aussi recevoir un PNG, JPG ou SVG depose, avec reglage d'opacite.
- Les blocs peuvent etre deplaces a la souris, avec les sliders X/Y ou les fleches du clavier.
- Options d'alignement : gauche, centre horizontal, droite, haut, centre vertical, bas, centrage complet et reset de l'element.

## Export PDF

Le bouton `PDF HD` génère un fichier aux dimensions de l’étiquette. L’export groupé crée une planche A4, A3 ou A5 optimisée, avec les marges et traits de coupe choisis. Le PNG utilise la formule `pixels = millimètres × 300 / 25,4`.

## IA
Outil créé à l'aide de codex pour plus d'infos, voir [PROMPT.md](PROMPT.md)
