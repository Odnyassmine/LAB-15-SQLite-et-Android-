# Gestion des Étudiants - Application Android (SQLite)

Cette application Android est un projet de gestion minimale des étudiants, démontrant l'utilisation d'une base de données SQLite embarquée pour effectuer des opérations CRUD (Create, Read, Update, Delete).

##Fonctionnalités

- **Ajout d'étudiants** : Saisie du nom et du prénom.
- **Recherche par ID** : Affichage des informations d'un étudiant à partir de son identifiant unique.
- **Suppression d'étudiants** : Retrait définitif d'un étudiant de la base de données via son ID.
- **Persistance locale** : Les données sont conservées localement dans une base SQLite nommée `ecole`.
- **Suivi Logcat** : Journalisation des opérations d'insertion et de suppression pour le débogage.

##Architecture du Projet

Le projet respecte une séparation claire des responsabilités :

- **`projet.fst.ma.app.classes`** : Contient le modèle métier `Etudiant`.
- **`projet.fst.ma.app.util`** : Contient `MySQLiteHelper`, gérant la création et la mise à jour de la base de données.
- **`projet.fst.ma.app.service`** : Contient `EtudiantService`, la couche d'accès aux données (DAO) implémentant le CRUD.
- **`projet.fst.ma.app`** : Contient la `MainActivity` (Couche présentation).

## Technologies utilisées

- **Langage** : Java
- **Base de données** : SQLite
- **UI** : XML Layouts (AppCompat / Material Components)
- **Minimum SDK** : API 24 (Android 7.0)

## Aperçu de l'interface

L'interface utilisateur simple permet de :
1. Saisir le **Nom** et le **Prénom**.
2. Cliquer sur **Valider** pour enregistrer.
3. Saisir un **ID Etudiant** pour **Chercher** ou **Supprimer**.

## ⚙️ Installation

1. Clonez le dépôt.
2. Ouvrez le projet dans **Android Studio**.
3. Synchronisez les fichiers Gradle.
4. Lancez l'application sur un émulateur ou un appareil physique.


