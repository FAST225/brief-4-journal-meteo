# Fiche individuelle

> Une page, avant la livraison. : 
**Prénom et nom** : abdul sobur titilope fakayode
**Compte GitHub** : FAST225


1. **Une fonction que j'ai écrite**, et comment elle marche : J'ai travaillé sur les fonctions de gestion des relevés météorologiques, notamment la fonction ajouterReleve() du fichier src/registre.js.

Objectif de la fonction :

Permettre l'ajout d'un nouveau relevé météorologique dans le tableau des relevés, après avoir vérifié que les informations saisies sont correctes.

Ses paramètres :

releves : le tableau contenant les relevés déjà enregistrés.

saisie : un objet contenant les nouvelles informations saisies par l'utilisateur (identifiant, date, température, pluie et humidité relative de l'air).

Son traitement :

Elle appelle verifierReleve() pour contrôler les informations saisies.
Si des erreurs sont détectées, elle les retourne sans modifier le tableau.
Si aucune erreur n'est détectée, elle appelle creerReleve() pour construire un nouvel objet avec les valeurs numériques.
Elle ajoute ce nouvel objet au tableau avec la méthode push().
Sa valeur de retour :
Un tableau contenant les messages d'erreur si la saisie est incorrecte.
Un tableau vide [] si l'ajout a réussi.

2. **Une difficulté, et sa solution** : difficulté : un problème de syntaxe JavaScript.

Le terminal affichait le message suivant :

file:///.../src/registre.js:15

avec une erreur signalée au niveau de l'instruction return.
Pour rechercher l'origine du problème, j'ai :
Localisé la ligne indiquée dans le message d'erreur.
Vérifié les accolades et les blocs conditionnels de la fonction.
Vérifié que le return se trouvait bien à l'intérieur de la fonction.
Comparé la structure de la fonction avec la syntaxe attendue.

3. **L'entraide** (qui m'a aidé, qui j'ai aidé, sur quoi) : KOUASSI ANGLOVIA m'a aide sur la recherche dans un tableau et la notion de MATH.max et MATH.min .
j'ai aidé Falle jaures,irie bi,Levi anoh,Ouedraogo Bourahima,Kouame Kouadio Florent,Brou Grace Emmanuella,Kone ABDOULAYE,...
