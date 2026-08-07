# Atelier d'etiquettes de potions

Webapp locale pour creer et editer des stickers de potions pour un cosplay.

## Utilisation

Ouvre `index.html` dans ton navigateur. L'app fonctionne sans installation.
C'est également disponible [ici](https://maelremrem.github.io/PotionStickers/)

## Nouveautes

- Rendu SVG vectoriel : les contours externes et internes suivent la decoupe.
- Dimensions libres en millimetres pour la largeur et la hauteur. Les exports PNG sont calcules a 300 dpi.
- Exports unitaires : PNG HD, SVG et PDF via la fenetre d'impression du navigateur.
- Liste de designs valides via le bouton `Ajouter a la liste des exports` pour preparer plusieurs etiquettes avant export groupe.
- Export groupe depuis une modal : ZIP de PNG HD, ZIP de PDF HD, ou un seul PDF avec tous les designs cote a cote avec 2 mm de marge.
- Plus d'exemples : Deadly Nightshade, Mermaid Tears, Love Potion, Elixir of Life, Phoenix Ashes, Moon Dust, Dragon's Breath, Basilisk Venom, Ghost Ink, Royal Antidote, Snail Slime, Vampire Tonic.
- Plus de formes : rectangle, arche, badge, diamant, blason, ticket.
- Plus de polices de titre et de symboles.
- Le numero et le flacon sont des champs texte libres.
- Le symbole central peut etre remplace par un PNG, JPG ou SVG depose.
- Le fond de l'etiquette peut aussi recevoir un PNG, JPG ou SVG depose, avec reglage d'opacite.
- Les blocs peuvent etre deplaces a la souris, avec les sliders X/Y ou les fleches du clavier.
- Options d'alignement : gauche, centre horizontal, droite, haut, centre vertical, bas, centrage complet et reset de l'element.

## Export PDF

Le bouton `PDF` ouvre une page d'impression au format indique dans les champs largeur/hauteur. Choisis `Enregistrer au format PDF` dans ton navigateur pour garder un fichier vectoriel net. Le PNG utilise la formule `pixels = millimetres x 300 / 25,4`.

## IA
Outil créé à l'aide de codex pour plus d'infos, voir [PROMPT.MD](PROMPT.MD)
