------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Décrivez les éléments de votre projet à l'aide de variables](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/911847-decrivez-les-elements-de-votre-projet-a-laide-de-variables)</p>

#### A. Comprenez ce qu'est une variable
###### 1. Donnez toujours un nom et une valeur aux variables
```php
DATE = 221012
HEURE = 1951
```
###### 2. Découvrez les différents types de variables
| Type   | Description           | Donnée                | 
| ------ | --------------------- | --------------------- |
| string | chaînes de caractères | Texte                 |
| int    | Nombre Entier         | 1 2 3 ou -1 -2 -3     |
| float  | Nombre avec virgule   | 14,5 30.2             |
| bool   | Vrai ou Faux          | true, false           |
| NULL   | Valeur NUL            |                       |


#### B. Affectez une valeur à une variable
###### 1. Définir une Variable à une valeur
```php
<?php
  $userAge = 17;
  echo $userAge
?>
```
Explication:
```
$       : Permet de définir une variable
userAge : Nom de la Variable
=       : Egale à
17      : Valeur de la variables
;       : Permet de conclure la valeur
```

#### C. Utilisez les types de données
###### 1. Le type string  (chaîne de caractères)
```php
<?php
  $fullname = "Mathieu Nebra";
  $email = 'mathieu.nebra@exemple.com';
  $prenom1 = "Mon \"nom\" est Mathieu";
  $prenom2 = 'Je m\'appelle Mathieu';
?>
```
###### 2. Le type int  (nombre entier)
```php
<?php
$userAge = 17;
?>
```
###### 3. Le type float  (nombre décimal)
```php
<?php
$price = 57.3;
?>
```
###### 4. Le type bool  (booléen)
```php
<?php
$isAuthor = true;
$isAdministrator = false;
?>
```
###### 5. Une variable vide avec NULL
```php
<?php
$noValue = NULL;
?>
```
#### D. Affichez le contenu d'une variable
###### 1. 
```php
  echo $email;
  echo $fullname;
  echo $prenom1;
  echo $prenom2;
  echo $isAuthor;
  echo $userAge;
  echo $price;
  echo $noValue;
```
#### E. Concaténez une variable

###### 1. Exemple
```php
<?php
$fullname = "Mathieu Nebra";
echo "Bonjour ";
echo $fullname;
echo " et bienvenue sur le site !";
?>
```
###### 2. Concaténez avec des guillemets doubles
```php
<?php
$fullname = "Mathieu Nebra";
echo "Bonjour $fullname et bienvenue sur le site !";
?>
```
###### 3. Concaténez avec des guillemets simples (Abend !!!)
```php
<?php
$fullname = 'Mathieu Nebra';
echo 'Bonjour $fullname et bienvenue sur le site !'; // ERREUR !
?>
```
Correctif:
```
<?php
$fullname = 'Mathieu Nebra';
echo 'Bonjour ' . $fullname . ' et bienvenue sur le site !'; // OK
?>
```
#### F. Faites des calculs simples
###### 1. Les opérations de base : addition, soustraction…
| Symbole | Signification  |
| ------- | -------------- |
|    +    | Addition       |
|    -    | Soustraction   |
|    *    | Multiplication |
|    /    | Division       |
|    %    | Modulo         |

**Exemple 1**
```php
<?php
$number = 2 + 4; // $number prend la valeur 6
$number = 5 - 1; // $number prend la valeur 4
$number = 3 * 5; // $number prend la valeur 15
$number = 10 / 2; // $number prend la valeur 5

// Allez on rajoute un peu de difficulté
$number = 3 * 5 + 1; // $number prend la valeur 16
$number = (1 + 2) * 2; // $number prend la valeur 6
?>
```
**Exemple 2**
```php
<?php
$number = 10;
$result = ($number + 5) * $number; // $result prend la valeur 150
?>
```
###### 2. Le modulo
Modulo représente le reste de la division entière.
Si la valeur est entier, elle retourne 0 sinon 1.
```php
<?php
$number = 10 % 5; // $number prend la valeur 0 car la division tombe juste
$number = 10 % 3; // $number prend la valeur 1 car il reste 1
echo $number 
?>
```


------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Adaptez le comportement de votre application à l'aide des conditions](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/912046-adaptez-le-comportement-de-votre-application-a-laide-des-conditions)</p>

#### A. Appropriez-vous la structure de base :  if… else
###### 1. Les symboles 
| Symbole | Signification           |
| ------- | ----------------------- |
|   ==    | Est égal à              |
|   >     | Est supérieur à         |
|   <     | Est inférieur à         |
|   >=    | Est supérieur ou égal à |
|   <=    | Est inférieur ou égal à |
|   !)    | Est différent de        |


###### 2. Utilisez la structure  if… else

###### IF
```php
<?php
$isEnabled = true;
if ($isEnabled == true) {
  echo "Vous êtes autorisé(e) à accéder au site ✅"; 
  }
?>
```

###### IF + ELSE
```php
<?php
$isEnabled = true;
if ($isEnabled == true) {
  echo "Vous êtes autorisé(e) à accéder au site ✅";
  }
else {
  echo "Accès refusé ❌ ";
  }
?>
```



###### 3. 
```html
```

###### 4. 
```html
```
















#### B. Utilisez la condition switch pour optimiser votre code
###### 1. 
```html
``` 
###### 2. 
```html
``` 
###### 3. 
```html
```
###### 4. 
```html
```
#### C. Découvrez les ternaires : des conditions condensées
###### 1. 
```html
``` 
###### 2. 
```html
``` 

###### 3. 
```html
```

###### 4. 
```html
```

------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> []()</p>
#### A.  
###### 1. 
```html
``` 
###### 2. 
```html
``` 

###### 3. 
```html
```

###### 4. 
```html
```

