----------------------------------------------------------------------------------------------------------------------------------------------------------------------

<p align='center'> Structure des tables SQL </p>

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### A. Création de la Base de ddonnée du site

##### 1. Suppression de la Database
```sql
DROP DATABASE IF EXISTS website;
```
##### 2. Création de la Database

```sql
CREATE DATABASE website;
```

##### 3. Modification de la Database
```sql
ALTER DATABASE website CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### B. config_website

|  TYPE    | Nom de l'objet     | Exemple de contenu        | Confirmer |
| -------- | ------------------ | ------------------------- | --------- |
| XXXXXX   | Name_Website       | Drthrax74                 |    NON    |
| XXXXXX   | Visible au public  | true                      |    NON    |


##### Supprimer la Table
```
DROP TABLE IF EXISTS config;
```

##### Création de la table
```
CREATE TABLE config
(
  name VARCHAR(100)  
);
```

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

### B. Table Users

| TYPE d'objet  | Nom de l'objet     | Exemple de contenu        | Confirmer |
| ------------- | ------------------ | ------------------------- | --------- |
| INT           | id                 | Primaire / AUTO_INCREMENT |    OUI    |
| VARCHAR(30)   | nom                | MyName                    |    NON    |
| VARCHAR(20)   | prenom             | MySurname                 |    NON    |
| VARCHAR(255)  | email              | support@support.com       |    NON    |
| DATE          | date_naissance     | 01-01-1998                |    NON    |
| VARCHAR(20)   | pays               | France                    |    NON    |
| VARCHAR(50)   | ville              | Lyon                      |    NON    |
| DATE          | Date d'inscription | 13-10-2022                |    NON    |
| DATE          | Dern. connexion    | 13-10-2022 04:00          |    NON    |
| VARCHAR(3)    | Age                | 18                        |    NON    |
| XXXXXX        | Compte activé      | true                      |    NON    |
| XXXXXX        | BANNIE             | false                     |    NON    |
| VARCHAR(20)   | Utilisateur        | MyUsername                |    NON    |
| XXXXXX        | Statut             | Super Admin               |    NON    |
| XXXXXX        | Mot de passe       | Passw0rd2022              |    NON    |
| VARCHAR(30)   | Informations       | Signature:                |    NON    |
| XXXXXX        | Permission         | Administrateurs           |    NON    |


##### Supprimer la Table
```
DROP TABLE IF EXISTS users;
```

##### Création de la table
```sql
CREATE TABLE users
(
  id INT PRIMARY KEY NOT NULL,
  nom VARCHAR(30),
  prenom VARCHAR(20),
  email VARCHAR(255),
  date_naissance DATE,
  pays VARCHAR(255),
  ville VARCHAR(255)
)
```

<br />


----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### C. Articles

| TYPE d'objet  | Nom de l'objet     | Exemple de contenu    | Confirmer |
| ------------- | ------------------ | --------------------- | --------- |
| XXXXXX        | titre_article      | Ouverture du site     |    NON    |
| XXXXXX        | contenu            | Bienvenue sur le site |    NON    |
| XXXXXX        | auteur             | MyUsername            |    NON    |
| XXXXXX        | date_de_postage    | 01-01-1998            |    NON    |
| XXXXXX        | heure_postage      | 04:00                 |    NON    |
| XXXXXX        | etat_publication   | true                  |    NON    |
