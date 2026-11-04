# Relevé des tests

> Écrivez le résultat attendu avant d'essayer. Un écart n'est pas une faute : notez-le, corrigez, refaites le test.

**Calculs à la main** :4
 - Températures : 27 + 28 + 26 + 29 + 27 + 30 + 28 + 26 + 29 + 30 = 280 °C-relevés. Moyenne : 280 / 10 = **28 °C**.
- Température minimale de la série : **26 °C** (M03 et M08).
- Température maximale de la série : **30 °C** (M06 et M10).
- Cumul de pluie : 0 + 5 + 12 + 0 + 3 + 0 + 8 + 15 + 0 + 2 = **45 mm**.
- Jours avec au moins 10 mm : **2** (M03 : 12 mm ; M08 : 15 mm).
**Essais dans le menu** : un ajout valide (encore là après redémarrage), chaque règle refusée, une recherche introuvable, chaque tri, la synthèse, un choix inconnu.


## Essais manuels  effectuer dans le terminal

Les essais suivants sont un protocole de vérification à jouer sur le poste de l'étudiant. Ne pas remplir « obtenu » avant de les avoir réellement exécutés.

| Action | Attendu | Obtenu | Testeur |
| --- | --- | --- | --- |
| Ajouter un relevé valide, quitter puis relancer | Le relevé est toujours présent après redémarrage | Le relevé est toujours présent après redémarrage effectivement | M11 | 2026-11-03 | 28 °C | 6 mm | air 76 % |

| Saisir une pluie négative | Saisie refusée, journal inchangé |Relevé refusé :
  - La pluie doit être un nombre positif ou nul (en mm), journal inchangé  |-12 |

| Saisir une humidité de 101 % | Saisie refusée, journal inchangé | Relevé refusé :
  - L'humidité relative de l'air doit être un nombre entre 0 et 100 (%),journal inchangé.| 101  |

| Rechercher la date `2026-10-22` | Le relevé M08 est affiché | Date (AAAA-MM-JJ) : 2026-10-22
M08 | 2026-10-22 | 26 °C | 15 mm | air 85 % | 2026-10-22 |

| Rechercher la date `2026-10-30` | Message indiquant que le relevé est introuvable | Date (AAAA-MM-JJ) : 2026-10-30
Relevé du 2026-10-30 introuvable. | 2026-10-30 |

| Trier par pluie | Les pluies apparaissent par ordre croissant, le journal initial reste inchangé | À exécuter | 2026-10-30 |

| Afficher la synthèse | 28 °C ; 26 °C ; 30 °C ; 45 mm ; 2 journées pluvieuses | M03 | 2026-10-17 | 26 °C | 12 mm | air 82 %
M08 | 2026-10-22 | 26 °C | 15 mm | air 85 %
M01 | 2026-10-15 | 27 °C | 0 mm | air 75 %
M05 | 2026-10-19 | 27 °C | 3 mm | air 80 %
M02 | 2026-10-16 | 28 °C | 5 mm | air 78 %
M07 | 2026-10-21 | 28 °C | 8 mm | air 76 %
M11 | 2026-11-03 | 28 °C | 6 mm | air 76 %
M04 | 2026-10-18 | 29 °C | 0 mm | air 70 %
M09 | 2026-10-23 | 29 °C | 0 mm | air 72 %
M06 | 2026-10-20 | 30 °C | 0 mm | air 68 %
M10 | 2026-10-24 | 30 °C | 2 mm | air 74 % | trier par temperature |

| Entrer un choix inconnu | Message de choix inconnu puis retour au menu | Choix inconnu : « 9 ». Tapez un chiffre du menu. | 9 |

|Faire une synthese de la serie| Afficher la synthese de la serie|--- Synthèse de la série ---
Nombre de relevés : 10
Température moyenne : 28 °C
Température minimale : 26 °C · maximale : 30 °C
Cumul de pluie : 45 mm
Journées avec au moins 10 mm de pluie : 2
Journée la plus chaude : M06 | 2026-10-20 | 30 °C | 0 mm | air 68 %
Rappels :
  - Quelques jours de relevés forment une courte série météo : ils ne décrivent pas le climat de la région.
  - Le seuil de 10 mm est une catégorie d’exercice : il ne prévoit ni inondation ni stress hydrique.
  - L'humidité relative de l'air (en %) n'est pas l'humidité du sol.|choix 5

|Suprimer un relevé|Le releve a étè supprimer,avec le journal à jour |Identifiant : M11
Relevé M11 supprimé. Le journal compte 10 relevé(s).|

|Modifier un releve|le releve a ete modifier| Modification refuser|id:M10,date:2026-10-05

**Sur un autre poste** (`git clone`, `node app.js`, `npm test`, en suivant le README) : ✏️
