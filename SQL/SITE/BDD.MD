----------------------------------------------------------------------------------------------------------------------------------------------------------------------

<p align='center'> Structure des tables SQL </p>

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### C. General

|  TYPE    | Nom de l'objet     | Exemple de contenu        | Confirmer |
| -------- | ------------------ | ------------------------- | --------- |
| string   | Name Website       | Drthrax74                 |    NON    |


----------------------------------------------------------------------------------------------------------------------------------------------------------------------

### B. Table Users

|  TYPE    | Nom de l'objet     | Exemple de contenu        | Confirmer |
| -------- | ------------------ | ------------------------- | --------- |
| int      | ID                 | Primaire / AUTO_INCREMENT |    OUI    |
| int      | Date d'inscription | 13-10-2022                |    NON    |
| int      | Dern. connexion    | 13-10-2022 04:00          |    NON    |
| int      | Date de Naissance  | 01-01-1998                |    NON    |
| int      | Age                | 18                        |    NON    |
| bool     | Compte activé      | true                      |    NON    |
| bool     | BANNIE             | false                     |    OUI    |
| string   | Utilisateur        | MyUsername                |    OUI    |
| string   | Statut             | Super Admin               |    OUI    |
| string   | Mot de passe       | Passw0rd2022              |    NON    |
| string   | Adresse EMAIL      | support@support.com       |    OUI    |
| string   | Nom                | MyName                    |    OUI    |
| string   | Prénom             | MySurname                 |    OUI    |
| string   | Informations       | Signature:                |    OUI    |
| string   | Permission         | Administrateurs           |    OUI    |

```sql
DROP TABLE users;


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
