# Mon vocabulaire chinois

Petit site de révision pour GitHub Pages : cartes à retourner avec calendrier de révision, liste consultable et formulaire pour ajouter des mots.

## Mise en ligne

1. Sur GitHub, crée un dépôt public (par exemple `chinois`).
2. Clique sur « Add file », puis « Upload files », et dépose `index.html`, `words.js` et ce `README.md`. Valide avec « Commit changes ».
3. Va dans Settings, puis Pages. Dans « Build and deployment », choisis « Deploy from a branch », la branche `main` et le dossier `/ (root)`, puis enregistre.
4. Au bout d'une minute environ, le site est disponible à l'adresse `https://TON-PSEUDO.github.io/chinois/`.

## Ajouter des mots

Il y a deux façons de faire, à combiner comme tu veux.

**Depuis le site.** Onglet « Ajouter » : remplis le formulaire (le pinyin peut être tapé avec des chiffres, `ni3 hao3` devient `nǐ hǎo`). Le mot est tout de suite disponible pour les révisions, mais il n'est enregistré que dans le navigateur utilisé. Pour le garder dans le site, clique sur « Télécharger words.js », puis remplace le fichier `words.js` du dépôt (Add file, Upload files, même nom de fichier).

**Directement sur GitHub.** Ouvre `words.js`, clique sur le crayon et ajoute une ligne avant le `];` final, en respectant la même forme :

```
 {"zh": "你好", "py": "nǐ hǎo", "fr": "bonjour", "ex": "", "expy": "", "exfr": "", "tag": "ajout", "check": false},
```

Pense à la virgule en fin de ligne. Mets `"check": true` pour afficher la mention « à vérifier » sur un mot dont tu doutes.

## Bon à savoir

- Les progrès de révision (cartes sues ou non) sont enregistrés dans le navigateur, séparément sur chaque appareil.
- Le bouton 🔊 utilise la voix chinoise de l'appareil, quand il en possède une.
- Le champ `tag` sert à filtrer : `page01` à `page15` correspondent aux pages de ton cahier, et tu peux inventer d'autres thèmes.
