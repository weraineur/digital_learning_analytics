# Digital Learning Analytics

Projet d'analyse de données pédagogiques issues de **Moodle Ecoris Online** pour identifier les modules à risque, suivre la performance des étudiants et orienter les décisions pédagogiques.

## Objectifs
- Mesurer la performance des étudiants par cours et par formation.
- Identifier les modules les plus difficiles.
- Suivre le taux de réussite et le taux d'abandon.
- Produire des indicateurs exploitables pour l'amélioration continue.

## Source de données
- Export CSV Moodle (rapports d'activité et de notes).

## Variables attendues
- Nom complet du cours
- Nom de l'utilisateur
- Note du cours
- Suivi des activités des participants (%)
- Statut d'achèvement (Oui/Non)
- Date/temps de participation
- Durée jusqu'à l'achèvement
- Modalité (présentiel / distanciel)

## KPI
- **Taux d'achèvement** = étudiants ayant terminé / étudiants inscrits
- **Durée médiane d'achèvement** par module
- **Note moyenne et note médiane** par module
- **Taux d'abandon** = étudiants non terminés / étudiants inscrits

## Segmentation de l'analyse
- Par module
- Par formation
- Par modalité (présentiel vs distanciel)

## Seuils d'alerte (version initiale)
- Taux d'achèvement < 60 %
- Note moyenne < 10/20
- Durée d'achèvement anormalement élevée (vs médiane globale)
- Taux d'abandon élevé (seuil à ajuster selon l'historique)

## Livrables attendus
- Tableaux des modules avec :
  - durée d'achèvement la plus longue,
  - plus fort taux de non-achèvement,
  - notes les plus faibles.
- Tableau de bord simple :
  - Top 10 modules à risque,
  - tendances temporelles des KPI,
  - comparatif présentiel/distanciel.

## Structure actuelle du dépôt
- `Projet Digital learning analytics.txt` : cadrage initial du projet
- `README.md` : présentation du projet

## Prochaines étapes
1. Préparer et nettoyer le fichier CSV Moodle.
2. Standardiser les types (notes, dates, booléens).
3. Calculer les KPI par module/formation/modalité.
4. Construire le tableau de bord.

## Auteur
- weraineur
