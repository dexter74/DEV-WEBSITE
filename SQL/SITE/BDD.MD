----------------------------------------------------------------------------------------------------------------------------------------------------------------------

<p align='center'> Structure des tables SQL </p>




----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### A. Création de la Base de ddonnée du site

##### Suppression de la Database
```sql
DROP DATABASE IF EXISTS website;
```
##### Création de la Database

```sql
CREATE DATABASE website  DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

##### Modification de la Database
```sql
ALTER DATABASE website CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### B. config_website

|  TYPE    | Nom de l'objet     | Exemple de contenu        | Confirmer |
| -------- | ------------------ | ------------------------- | --------- |
| string   | Name_Website       | Drthrax74                 |    NON    |
| bool     | Visible au public  | true                      |    NON    |

```
DROP TABLE IF EXISTS config;
CREATE TABLE config
(
  name VARCHAR(100)
  
);
```





----------------------------------------------------------------------------------------------------------------------------------------------------------------------

### B. Table Users

|  TYPE    | Nom de l'objet     | Exemple de contenu        | Confirmer |
| -------- | ------------------ | ------------------------- | --------- |
| int      | id                 | Primaire / AUTO_INCREMENT |    OUI    |
| string   | nom                | MyName                    |    NON    |
| string   | prenom             | MySurname                 |    NON    |
| string   | email              | support@support.com       |    NON    |
| int      | date_naissance     | 01-01-1998                |    NON    |
| int      | pays               | France                    |    NON    |
| int      | ville              | Lyon                      |    NON    |


| int      | Date d'inscription | 13-10-2022                |    NON    |
| int      | Dern. connexion    | 13-10-2022 04:00          |    NON    |
| int      | Age                | 18                        |    NON    |
| bool     | Compte activé      | true                      |    NON    |
| bool     | BANNIE             | false                     |    NON    |
| string   | Utilisateur        | MyUsername                |    NON    |
| string   | Statut             | Super Admin               |    NON    |
| string   | Mot de passe       | Passw0rd2022              |    NON    |
| string   | Informations       | Signature:                |    NON    |
| string   | Permission         | Administrateurs           |    NON    |

```sql
CREATE TABLE users
(
  id INT PRIMARY KEY NOT NULL,
  nom VARCHAR(100),
  prenom VARCHAR(100),
  email VARCHAR(255),
  date_naissance DATE,
  pays VARCHAR(255),
  ville VARCHAR(255)
)
```


<br />


----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### C. Articles

|  TYPE    | Nom de l'objet        | Exemple de contenu    | Confirmer |
| -------- | --------------------- | --------------------- | --------- |
| string   | Titre de l'article    | Ouverture du site     |    OUI    |
| string   | Contenue de l'article | Bienvenue sur le site |    OUI    |
| string   | Auteur                | MyUsername            |    OUI    |
| int      | Date de postage       | 01-01-1998            |    NON    |
| int      | Heure postage         | 04:00                 |    NON    |
