-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Décrivez les éléments de votre projet à l'aide de variables](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/911847-decrivez-les-elements-de-votre-projet-a-laide-de-variables)</p>

### A. Comprenez ce qu'est une variable
#### 1. Donnez toujours un nom et une valeur aux variables
```php
$DATE = 221012
$HEURE = 1951
```
#### 2. Découvrez les différents types de variables
| Type   | Description           | Donnée                          | 
| ------ | --------------------- | ------------------------------- |
| string | chaînes de caractères | Texte                           |
| int    | Nombre Entier         | 1 2 3 ou -1 -2 -3               |
| float  | Nombre avec virgule   | 14,5 30.2                       |
| bool   | Vrai ou Faux          | true, false (Pas de Parenthèse) |
| NULL   | Valeur NULL           |                                 |

<br />

### B. Affectez une valeur à une variable
#### 1. Définir une Variable à une valeur
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

<br />

### C. Utilisez les types de données
#### 1. Le type string  (chaîne de caractères)
```php
<?php
  $fullname = "Mathieu Nebra";
  $email = 'mathieu.nebra@exemple.com';
  $prenom1 = "Mon \"nom\" est Mathieu";
  $prenom2 = 'Je m\'appelle Mathieu';
?>
```
#### 2. Le type int  (nombre entier)
```php
<?php
	$userAge = 17;
?>
```
#### 3. Le type float  (nombre décimal)
```php
<?php
	$price = 57.3;
?>
```
#### 4. Le type bool  (booléen)
```php
<?php
?>
```
#### 5. Une variable vide avec NULL
```php
<?php
	$isAuthor = true;
	$isAdministrator = false;
	$noValue = NULL;
?>
```

<br />

### D. Affichez le contenu d'une variable
```php
<?php
	echo $email;
	echo $fullname;
	echo $prenom1;
	echo $prenom2;
	echo $isAuthor;
	echo $userAge;
	echo $price;
	echo $noValue;
?>
```

<br />

### E. Concaténez une variable
#### 1. Exemple
```php
<?php
	$fullname = "Mathieu Nebra";
	echo "Bonjour ";
	echo $fullname;
	echo " et bienvenue sur le site !";
?>
```
#### 2. Concaténez avec des guillemets doubles
```php
<?php
	$fullname = "Mathieu Nebra";
	echo "Bonjour $fullname et bienvenue sur le site !";
?>
```
#### 3. Concaténez avec des guillemets simples 

##### Ecriture sans erreur 
Il faut des Points .
```php
<?php
	$fullname = 'Mathieu Nebra';
	echo 'Bonjour ' . $fullname . ' et bienvenue sur le site !'; // OK
?>
```

##### Ecriture avec une erreur
```php
<?php
	$fullname = 'Mathieu Nebra';
	echo 'Bonjour $fullname et bienvenue sur le site !'; // ERREUR !
?>
```


<br />

### F. Faites des calculs simples
#### 1. Les opérations de base : addition, soustraction…
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
#### 2. Le modulo
Modulo représente le reste de la division entière.
Si la valeur est entier, elle retourne 0 sinon 1.
```php
<?php
	$number = 10 % 5; // $number prend la valeur 0 car la division tombe juste
	$number = 10 % 3; // $number prend la valeur 1 car il reste 1
	echo $number 
?>
```

<br />

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Adaptez le comportement de votre application à l'aide des conditions](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/912046-adaptez-le-comportement-de-votre-application-a-laide-des-conditions)</p>

### A. Appropriez-vous la structure de base :  if… else
#### 1. Les symboles 
| Symbole | Signification           |
| ------- | ----------------------- |
|   ==    | Est égal à              |
|   >     | Est supérieur à         |
|   <     | Est inférieur à         |
|   >=    | Est supérieur ou égal à |
|   <=    | Est inférieur ou égal à |
|   !)    | Est différent de        |

<br />

#### 2. Utilisez la structure  if… else
##### Si
```php
<?php
	$isEnabled = true;
	if ($isEnabled == true) {echo "Vous êtes autorisé(e) à accéder au site ✅";}
?>
```
##### SI + SINON
```php
<?php
	$isEnabled = true;
	if ($isEnabled == true) {echo "Vous êtes autorisé(e) à accéder au site ✅";}
	else {echo "Accès refusé ❌ ";}
?>
```
##### SI + SINON + SINON SI
```php
<?php
	$ACCES = "AUTORISER";
	if ($ACCES == NULL) {echo "La valeur est Video";}
	elseif ($ACCES == "AUTORISER") {echo "Accès Autorisé";}
	elseif ($ACCES == "REFUSER") {echo "Accès refusé";}
	else {echo "Code retour en abend";}
?>
```
##### SI c'est vrai
```php
<?php
	$ACCESS = true;
	if ($ACCESS){echo "Accès autorisé";}
	else {echo "Accès refusé";}
?>
```

##### SI c'est faux
```php
<?php
	$ACCESS = false;
	if (! $ACCESS){echo "Accès refusé";}
	else{echo "???";}
?>
```











<br />

#### 3. Posez des conditions multiples
| Mot-clé | Signification | Symbole équivalent |
| ------- | ------------- | ------------------ | 
| AND     | Et            | &&                 |
| OR      | Ou            |  \|\|              | 
##### AND
```php
<?php
	$ACTIF = true;
	$AUTEUR = true;
	if ($ACTIF && $AUTEUR) {echo "Accès Autorisé! ✅";}
	else {echo"Accès refusé! ❌";}
?>
```
##### Multi-condition
```php
<?php
	$BYPASS = false;
	$USER   = 'Marc'; 
	$ADMIN  = true;
	$ETAT   = '1';
	$OK     = '✅';
	$KO     = '❌';
	echo "<b>Accès à l'administration: </b>";
	if(($BYPASS == 'true') || ($USER == 'Marc' && $ADMIN == 'true' && $ETAT == '1'))  {echo $OK;} else{echo $KO;}
?>
```


<br />

#### 4. Utilisez cette astuce bonus
##### Méthode 1
```php
<?php
// Variable
$chickenRecipesEnabled = true;

//SI
if ($chickenRecipesEnabled) {echo '<h1>Liste des recettes à base de poulet</h1>';}
?>
```
##### Méthode 2
```php
// Variable
<?php $chickenRecipesEnabled = true; ?>

//SI (Ne pas oublier le :)
<?php if ($chickenRecipesEnabled): ?>

//Phrase à afficher
<h1>Liste des recettes à base de poulet</h1>

//Fin de la condition (Ne pas oublier le ;)
<?php endif; ?>
```

<br />

### B. Utilisez la condition switch 
`/!\ Le switch ne peut tester que l'égalité`

`L'instruction break  demande à PHP de sortir du switch`


##### 1. Différentes écritures
##### Méthode if elseif else
```php
<?php
$grade = 16;
if ($grade == 0) {echo "Tu es vraiment un gros nul !!!";}
elseif ($grade == 5) {echo "Tu es très mauvais";}
elseif ($grade == 16) {echo "Tu te débrouilles très bien !";}
elseif ($grade == 20) {echo "Excellent travail, c'est parfait !";}
else {echo "Désolé, je n'ai pas de message à afficher pour cette note";}
?>
```
##### Méthode Swtich
```php
<?php
$grade = 1;

switch ($grade)
{ 
    case 0:
        echo "Tu es vraiment un gros nul !!!";
    break;

    case 1:
        echo "Tu as pile poil la moyenne, c'est un peu juste…";
    break;

    case 3:
        echo "Excellent travail, c'est parfait !";
    break;

    default:
        echo "Désolé, je n'ai pas de message à afficher pour cette note";
}
?>
```

<br />

#### C. Découvrez les ternaires : des conditions condensées
##### 1. Présentation
```
Un ternaire est une condition condensée qui sert à faire deux choses sur une seule ligne :
Tester la valeur d'une variable dans une condition.
Affecter une valeur à une variable selon que la condition est vraie ou non.
```
#### 2. Exemples
##### Méthode 1
```php
<?php

// Variable
$userAge = 24;

// Si
if ($userAge >= 18) {$isAdult = true;}

// SINON
else {$isAdult = false;}

// Message de sorti
if ($isAdult){echo "L'utilisateur est un adulte"}
?>
``` 
##### Méthode 2
```php
<?php

// Variable
$userAge = 24;

// Vérification
$isAdult = ($userAge >= 18) ? true : false;

// Ou mieux, dans ce cas précis
$isAdult = ($userAge >= 18);

// Message de sorti
if ($isAdult){echo "L'utilisateur est un adulte"}

?>
```

<br />

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Affichez une liste de recettes à l'aide des boucles](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/912133-affichez-une-liste-de-recettes-a-laide-des-boucles)</p>

### A. Utilisez un tableau pour lister des éléments
```
Pour crée un tableau, il faut déclarer les données du tableau $TEST = ['<Contenu de l'indice 0>','<Contenu de l'indice 1>'];
Ensuite il faut déclarer les indices echo $TEST[<indice>]
```
#### 1. Création d'un tableau
```php
<?php

//Variable
$user1 = ['Mickaël Andrieu', 'email', 'S3cr3t', '34'];

//Tableau
echo $user1[0];
echo $user1[1];
echo $user1[2];
echo $user1[3];

?>
```

#### 2. Création d'un tableau d'un tableau  
```php
<?php
// Tableau des correspondances
$user0 = ['20','Dexter74','Passw0rd2022','Jaques','levin','31','dexter74@mail.com','users'];
$user1 = ['21','Drthrax74','Passw0rd2022','Paul','courrier','31','drthrax74@mail.com','Administrateur'];

// Tableau regroupant les correspondances
$users = [$user0, $user1];

// Interroge le tableau regroupant
echo $users[0][0] . ' | '; // 20
echo $users[0][1] . ' | '; // Dexter74
echo $users[0][6] . ' | '; // dexter74@mail.com
echo '<br />';
echo $users[1][0] . ' | '; // 21
echo $users[1][1] . ' | '; // Drthrax74
echo $users[1][6] . ' | '; // drthrax74@mail.com
?>
```

<br />

### B. Utilisez une boucle simple :  while
```
Les instructions sont lancés dans l'ordre de haut en bas.
puis la boucle relance le processus à l'infini sauf si elle est conditionnée.
```

<p align='center'> <img src='https://user-images.githubusercontent.com/35907/195477079-0de95ec5-2a31-4821-9023-64d014598c29.png'> </p>



##### Boucle Infini
```php
<?php

//Tant que $TEST est vrai: 
while ($TEST) {echo "Mon Message qui se répéte à l'infini <br />";}

?>
```

##### La Boucle qui se répète X fois avec incrémentation
```php
<?php

// Variable
$LIGNE = 1;

// Message + Incrémentation
while ($LIGNE <= 10){echo 'Le numéro de la ligne est . $lines . <br />'; $LIGNE++;}

?>
```

<br />


### C. Découvrez une boucle plus complexe :  for
`for  et while  donnent le même résultat et servent à la même chose : répéter des instructions en boucle`

#### 1. Exemple 1
```php
<?php
// Initiation + condition de bouclage et incrémentation à chaque boucle 
for ($lines = 0; $lines <= 2; $lines++) {echo $users[$lines][0] . ' ' . $users[$lines][1] . '<br />';}
?>
```
#### 2. Choisir For ou While
```
while  est plus simple et plus flexible : on peut faire tous les types de boucles avec, mais on peut oublier de faire certaines étapes, comme l'incrémentation de la variable.
for  est bien adapté quand on doit compter le nombre de fois que l'on répète les instructions, et il permet de ne pas oublier de faire l'incrémentation pour augmenter la valeur de la variable !

Est-ce que je sais d'avance combien de fois je veux que mes instructions soient répétées ? 
Si oui: for
Si Non: while
```

<br />

### D. Affichez des recettes
#### 1. Complex (Possiblement une erreur sur le résultat)
```php
<?php

// // Déclaration du tableau (Non numérotés)
$BDD = [
  ['20','Dexter74','Passw0rd2022','Jaques','Levin','31','dexter74@mail.com','users'],
  ['21','Drthrax74','Passw0rd2022','Paul','Courrier','31','drthrax74@mail.com','Administrateur'],
  ['22','Snake','Passw0rd2022','Alain','Charles','31','drthrax74@mail.com','Administrateur'],
  ];

// Lecture de la ligne 0 à 1 du tableau
for ($LIGNE = 0; $BDD <= 1; $BDD++){echo "Utilisateur: '. $BDD[$LIGNE][2] .' ('. $BDD[$LIGNE][7] .')"}
?>
```


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Organisez vos données à l'aide des tableaux](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/4238931-organisez-vos-donnees-a-laide-des-tableaux)</p>

### A. Familiarisez-vous avec les tableaux numérotés
#### 1. Tableau (Array)
La variable Array prend la valeur de la case du tableau sur laquel elle traite.

Dans le cas de la Colonne ID, elle aura comme valeur un numéro.

#### 2. Construisez un tableau numéroté
###### Tableau de Base
| ID | VALEUR      |
| -- | ----------- |
| 0  | Jean-Claude |
| 1  | Halidi      |
| 2  | Luc         |
| 3  | Marc        |

###### Construire un Tableau Numéroté
```php
<?php

// Déclaration d'un Tableau (Non numérotés)
$VALEUR0 = ['Jean-Claude', 'Halidi', 'Luc', 'Marc'];

// Déclaration d'un tableau indexé numériquement
$VALEUR1 = array('Jean-Claude', 'Halidi', 'Luc', 'Marc');
?>
```


<br />

--------------------------------------------------------
### B. Familiarisez-vous avec les tableaux associatifs
#### 1. 
```php
```
#### 2. 
```php
```
#### 3. 
```php
```
#### 4. 
```php
```

<br />

--------------------------------------------------------
### C. Parcourez un tableau
#### 1. 
```php
```
#### 2. 
```php
```
#### 3. 
```php
```
#### 4. 
```php
```

<br />

--------------------------------------------------------
### D. Recherchez dans un tableau
#### 1. 
```php
```
#### 2. 
```php
```
#### 3. 
```php
```
#### 4. 
```php
```

<br />


--------------------------------------------------------
### E. Affichez des recettes (version 2 !)
#### 1. 
```php
```
#### 2. 
```php
```
#### 3. 
```php
```
#### 4. 
```php
```

<br />


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> []()</p>
### A. 
#### 1. 
```php
```
#### 2. 
```php
```
#### 3. 
```php
```
#### 4. 
```php
```

<br />

### B. 
#### 1. 
```php
```
#### 2. 
```php
```
#### 3. 
```php
```
#### 4. 
```php
```

<br />

### C. 
#### 1. 
```php
```
#### 2. 
```php
```
#### 3. 
```php
```
#### 4. 
```php
```

<br />
