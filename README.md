# Journal météorologique de la ferme

> Projet individuel du SAS DFS, brief 4 (sujet : [SUJET.md](SUJET.md)). Remplacez chaque ✏️ par votre texte, puis supprimez cette ligne.

## Contexte
Le responsable de la ferme pédagogique et les techniciens qui suivent les activités agricoles utilisent ce journal pour conserver et consulter les observations météorologiques. L'utilisateur peut saisir une observation quotidienne comprenant une température, une quantité de pluie et l'humidité relative de l'air, puis retrouver un relevé, classer les observations et obtenir des statistiques sur la période disponible. Un relevé décrit la météo d'une journée ; les dix relevés fournis forment une courte série météorologique. Cette série ne suffit pas à caractériser le climat d'une région, qui s'étudie sur une longue période, généralement avec des normales climatiques calculées sur 30 ans. L'humidité enregistrée est celle de l'air et non celle du sol.


## Prérequis et lancement

- Node.js 20 ou plus récent, Git ; aucune bibliothèque à installer.

```bash
git clone https://github.com/VOTRE-COMPTE/brief-4-journal-meteo.git
cd brief-4-journal-meteo
node app.js
npm test
```

Sous PowerShell, si `npm` est bloqué : `npm.cmd test`.

## Fonctionnalités

✏️ *Cochez seulement ce qui marche : `- [x]`.*

- [x] Lire les relevés au démarrage et enregistrer les modifications dans `donnees/releves.json`.
- [x] Ajouter un relevé après validation des cinq champs.
- [x] Lister les relevés et signaler un journal vide.
- [x] Rechercher par identifiant ou par date.
- [x] Afficher les journées ayant reçu au moins 10 mm de pluie.
- [x] Trier par température croissante et par pluie croissante.
- [x] Calculer la moyenne, le minimum, le maximum des températures et le cumul des pluies.
- [x] Afficher les rappels sur la courte série, le seuil pédagogique et l'humidité de l'air.
- [x] Bonus : supprimer ou modifier un relevé.
- [x] Bonus : trier par température décroissante et trouver la journée la plus chaude.


## Données

Les données de départ sont des exemples fictifs stockés dans `donnees/releves.json`. Chaque relevé contient cinq champs : `id` (identifiant unique), `date` (format `AAAA-MM-JJ`), `temperatureC` (°C), `pluieMm` (mm) et `humiditeAirPct` (humidité relative de l'air, en %). Les règles et exemples sont détaillés dans [le dictionnaire des données](docs/dictionnaire-donnees.md).

Avec les dix observations de départ (du 15 au 24 octobre 2026), les résultats de référence sont : température moyenne 28 °C, minimum 26 °C, maximum 30 °C, cumul de pluie 45 mm et deux journées avec au moins 10 mm de pluie.


## Limites

- Dix jours constituent une courte série et ne permettent pas de décrire le climat de la région.
- Le seuil de 10 mm est une catégorie de l'exercice ; il ne constitue pas une prévision d'inondation ou de stress hydrique.
- L'humidité relative de l'air ne renseigne pas sur l'humidité du sol.
- Le programme vérifie le format et les valeurs des relevés, mais ne contrôle pas que les dates sont consécutives, sans doublon ni trou.
- Les données de départ sont fictives et ne doivent pas être utilisées comme observations agricoles réelles.

## Documents

[Dictionnaire des données](docs/dictionnaire-donnees.md) · [Tâches](docs/taches.md) · [Relevé des tests](docs/releve-tests.md) · [Journal de recherche](docs/journal-recherche.md) · [Fiche agronomique](docs/fiche-agronomique.md) · [Fiche individuelle](docs/fiche-individuelle.md)

## Auteur

ABDUL SOBUR TITILOPE FAKAYODE, compte FAST225. Entraide : BOURAHIMA OUEDRAOGO, SUR LES SUR MON ORDINATEUR ET LE DEPOT CLONER.*
