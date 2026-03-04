# 🎓 Gestion Universitaire — SQL / PostgreSQL

Modélisation et interrogation d'une base de données universitaire, développée dans le cadre d'un projet de L2 Informatique.

## 📋 Description

Ce projet met en place une base de données relationnelle pour gérer les étudiants, enseignants, cours, inscriptions et examens d'une université. Il couvre la modélisation (MCD), la création des tables et l'écriture de requêtes SQL avancées.

## 📁 Fichiers

| Fichier | Description |
|---|---|
| `MCD.pdf` | Modèle Conceptuel de Données |
| `Tables.sql` | Création des tables et contraintes (clés primaires, étrangères) |
| `insertion.sql` | Données de test |
| `requetes.sql` | 41 requêtes SQL d'interrogation |

## 🗂️ Modèle de données

La base contient 6 tables :

- **Etudiant** — informations personnelles des étudiants
- **Enseignant** — informations des enseignants et leur titre
- **Cours** — matière, salle, horaire et enseignant responsable
- **Inscription** — lien entre étudiant et cours (statut, semestre)
- **Examen** — examens associés à un cours
- **Evalue** — notes des étudiants aux examens

## 🔍 Requêtes couvertes

Les 41 requêtes abordent notamment :

- Sélections simples et filtres
- Jointures multiples (`JOIN`, `LEFT JOIN`)
- Agrégations (`COUNT`, `AVG`, `MAX`)
- Conditions sur groupes (`HAVING`)
- Sous-requêtes corrélées et non corrélées
- Calcul de taux de réussite et évolution entre semestres
- Répartition par tranche d'âge (`CASE`)

## 🚀 Exécution

Les scripts doivent être exécutés **dans cet ordre** sous PostgreSQL :

```sql
-- 1. Créer les tables
\i Tables.sql

-- 2. Insérer les données
\i insertion.sql

-- 3. Lancer les requêtes
\i requetes.sql
```

Ou via **pgAdmin** : ouvrir chaque fichier et l'exécuter dans l'ordre ci-dessus.

## 🛠️ Technologies

- **PostgreSQL**
- **SQL** (DDL, DML, DQL)

## 👨‍💻 Auteur

Projet réalisé en L3 MIAGE — BARRY Oumou Bailo