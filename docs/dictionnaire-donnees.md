# Dictionnaire des données

> Un champ par ligne, d'après `SUJET.md` et le fichier de `donnees/`. La première ligne sert de modèle.

| Champ | Signification | Type dans le JSON | Règle de validation | Unité | Exemple |
| --- | --- | --- | --- | --- | --- |
| `id` | Identifiant unique du relevé | Texte (chaîne) | Obligatoire et absent des identifiants déjà enregistrés | — | `M08` |
| `date` | Jour de l'observation | Texte (chaîne) | Date réelle au format `AAAA-MM-JJ` | — | `2026-10-22` |
| `temperatureC` | Température de l'air observée pour la journée | Nombre | Nombre fini ; valeur négative, nulle ou décimale acceptée | °C | `26` |
| `pluieMm` | Hauteur de précipitations mesurée | Nombre | Nombre fini positif ou nul | mm | `15` |
| `humiditeAirPct` | Humidité relative de l'air | Nombre | Nombre fini compris entre 0 et 100, bornes incluses | % | `85` |

**Listes de valeurs autorisées** : les identifiants sont des chaînes non vides et uniques ; les dates doivent exister au calendrier et respecter le format indiqué ; les trois mesures sont des nombres. La température peut être négative. La pluie ne peut pas être négative. L'humidité relative de l'air est comprise entre 0 et 100 %

**Sources** :  `SUJET.md`, `donnees/releves.json` et les règles de validation de `src/registre.js`.
