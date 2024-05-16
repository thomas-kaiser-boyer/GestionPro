# GestionPro - Application web de gestion d'entreprise

Ce projet est une application web de gestion d'entreprise, permettant de gérer la base de données clients et fournisseurs, le stock de produits, les commandes et factures, ainsi que la comptabilité.

### Le contenu de ce repository sera bientôt publié. Merci de votre patience.

## Stack technique

Back-end : Spring Boot
Front-end : React
Base de données : MariaDB

## Installation

Pour installer et lancer l'application, suivez les étapes suivantes :

### Clonez le repository GitHub :

`git clone https://github.com/thomas-kaiser-boyer/GestionPro.git`

### Installez les dépendances front-end :

```
cd [nom_projet]
npm install
```
### Installez les dépendances back-end :
```
cd backend
mvn clean install
```
### Lancez la base de données MariaDB :
```
sudo service mysql start
```
### Créez la base de données et importez les données d'exemple :
```
mysql -u root -p
CREATE DATABASE GestionPro;
USE GestionPro;
SOURCE /path/to/GestionPro/backend/src/main/resources/data.sql;
```
### Lancez l'application back-end :
```
cd [nom_projet]/backend
mvn spring-boot:run
```
### Lancez l'application front-end :
```
cd [nom_projet]
npm start
```
### L'application devrait maintenant être accessible à l'adresse suivante : http://localhost:3000/

## Fonctionnalités

Gestion de la base de données clients et fournisseurs, avec la possibilité de créer, d'éditer et de supprimer des fiches.
Gestion du stock de produits, avec la possibilité de suivre les entrées et les sorties, ainsi que les niveaux de stock.
Gestion des commandes et des factures, avec la possibilité de créer, d'éditer et de supprimer des documents, ainsi que de suivre leur statut.
Gestion de la comptabilité, avec la possibilité de saisir et de suivre les écritures comptables, ainsi que de générer des états financiers.
