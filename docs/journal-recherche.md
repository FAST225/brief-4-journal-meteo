# Journal de recherche

> Chaque recherche utile : ce que vous cherchiez, où (cours, [MDN](https://developer.mozilla.org/fr/docs/Web/JavaScript), [Node.js](https://nodejs.org/api/), un camarade, une IA…), ce que vous avez compris. Ce que vous gardez, vous devez pouvoir l'expliquer.
| Ce que je cherchais | Où consulter | Ce que je dois comprendre / vérifier | Utilisé dans |
| --- | --- | --- | --- |
| Lire et écrire un fichier de manière asynchrone | Documentation Node.js, module `node:fs/promises` (`readFile`, `writeFile`) | `await` attend la promesse ; `readFile` lit du texte ; `writeFile` écrit le fichier | `src/stockage.js` |
| Transformer du JSON en objet et inversement | MDN JavaScript, `JSON.parse()` et `JSON.stringify()` | `parse` transforme une chaîne JSON en données ; `stringify` produit une chaîne JSON ; le troisième argument permet l'indentation | `src/stockage.js` |
| Rechercher et filtrer dans un tableau | MDN JavaScript, `find()` et `filter()` | `find` renvoie le premier élément correspondant ; `filter` renvoie un nouveau tableau | `src/registre.js`, `src/recherche.js` |
| Trier une copie de tableau | MDN JavaScript, `sort()` et l'opérateur de décomposition | Le comparateur numérique définit l'ordre ; copier avec `[...tableau]` évite de modifier le tableau original | `src/recherche.js`, `src/bonus.js` |
| Calculer une somme et une moyenne | MDN JavaScript, `reduce()`, `Math.min()` et `Math.max()` | `reduce` accumule une valeur ; vérifier le cas du tableau vide avant une moyenne ou un minimum/maximum | `src/synthese.js` |
| Gérer les erreurs et les saisies terminal | Documentation Node.js et lecture de `src/saisie.js` | `try/catch` intercepte une erreur ; `null` indique que la saisie est fermée | `app.js` |
| Comprendre et expliquer les fonctions produites avec une aide IA | Assistant IA (ChatGPT), à confronter aux consignes et à la documentation officielle | Réexpliquer chaque fonction, vérifier les cas limites et ne garder que le code que je comprends | Tous les modules concernés |

**Liens utiles** : [MDN JavaScript](https://developer.mozilla.org/fr/docs/Web/JavaScript) · [Documentation Node.js](https://nodejs.org/api/).

