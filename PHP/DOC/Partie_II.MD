-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Décrivez les éléments de votre projet à l'aide de variables](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/911847-decrivez-les-elements-de-votre-projet-a-laide-de-variables)</p>

### A. Comprenez ce qu'est une variable
#### 1. Donnez toujours un nom et une valeur aux variables
```php
$DATE  = 221012
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
	$fullname = 'Mathieu Nebra';
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
	$isAuthor = true;
	$isAdministrator = false;
?>
```
#### 5. Une variable vide avec NULL
```php
<?php
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
	$fullname = 'Mathieu Nebra';
	echo 'Bonjour ';
	echo $fullname;
	echo ' et bienvenue sur le site !';
?>
```
#### 2. Concaténez avec des guillemets doubles
```php
<?php
	$fullname = 'Mathieu Nebra';
	echo 'Bonjour $fullname et bienvenue sur le site !';
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
	$number = 2 + 4;  // $number prend la valeur 6
	$number = 5 - 1;  // $number prend la valeur 4
	$number = 3 * 5;  // $number prend la valeur 15
	$number = 10 / 2; // $number prend la valeur 5

	// Allez on rajoute un peu de difficulté
	$number = 3 * 5 + 1;   // $number prend la valeur 16
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
	if ($isEnabled == true) {echo 'Vous êtes autorisé(e) à accéder au site ✅';}
?>
```
##### SI + SINON
```php
<?php
	$isEnabled = true;
	if ($isEnabled == true) {echo 'Vous êtes autorisé(e) à accéder au site ✅';}
	else {echo 'Accès refusé ❌ ';}
?>
```
##### SI + SINON + SINON SI
```php
<?php
	$ACCES = 'AUTORISER';
	if ($ACCES == NULL) {echo 'La valeur est Video';}
	elseif ($ACCES == 'AUTORISER') {echo 'Accès Autorisé!';}
	elseif ($ACCES == 'REFUSER')   {echo 'Accès refusé!';}
	else {echo 'Code retour en abend';}
?>
```
##### SI c'est vrai
```php
<?php
	$ACCESS = true;
	if ($ACCESS) {echo 'Accès autorisé';}
	else {echo 'Accès refusé';}
?>
```

##### SI c'est faux
```php
<?php
	$ACCESS = false;
	if (! $ACCESS) {echo 'Accès refusé';}
	else{echo 'Accès autorisé';}
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
	if ($ACTIF && $AUTEUR) {echo 'Accès Autorisé! ✅';}
	else {echo 'Accès refusé! ❌';}
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
##### Méthode 
```php
<?php
	$chickenRecipesEnabled = true;
	if ($chickenRecipesEnabled) {echo '<h1>Liste des recettes à base de poulet</h1>';}
?>
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
	if ($grade == 0) {echo 'Tu es vraiment un gros nul !!!';}
	elseif ($grade == 5) {echo 'Tu es très mauvais';}
	elseif ($grade == 16) {echo 'Tu te débrouilles très bien !';}
	elseif ($grade == 20) {echo 'Excellent travail, c'est parfait !';}
	else {echo 'Désolé, je n'ai pas de message à afficher pour cette note';}
?>
```

##### Méthode Swtich
```php
<?php
	$grade = 1;
	
	switch ($grade)
	{ 
	    case 0:
		echo 'Tu es vraiment un gros nul !!!';
	    break;

	    case 1:
		echo 'Tu as pile poil la moyenne, c'est un peu juste…';
	    break;

	    case 3:
		echo 'Excellent travail, c'est parfait !';
	    break;

	    default:
		echo 'Désolé, je n'ai pas de message à afficher pour cette note';
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
	echo $user1[0]; // Mickaël Andrieu
	echo $user1[1]; // email
	echo $user1[2]; // S3cr3t
	echo $user1[3]; // 34
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
	$CHECK = true;
	while ($CHECK) {echo 'Mon Message qui se répéte à l\'infini <br />';}
?>
```

##### La Boucle qui se répète X fois avec incrémentation
```php
<?php
	$LIGNE= 1;
	while($LIGNE <= 5){echo '<b>Numéro de ligne:</b> ' . $LIGNE . '<br />' ;$LIGNE++;}
?>
```

<br />


### C. Découvrez une boucle plus complexe :  for
`for  et while  donnent le même résultat et servent à la même chose : répéter des instructions en boucle`

#### 1. Exemple 1
```php
<?php
	// Tableau des correspondances
	$user0 = ['20','Dexter74','Passw0rd2022','Jaques','levin','31','dexter74@mail.com','users'];
	$user1 = ['21','Drthrax74','Passw0rd2022','Paul','courrier','31','drthrax74@mail.com','Administrateur'];
	$users = [$user0, $user1];

	// Afficher les lignes 0 et 1 sur la colonnes 0 et 1
	for ($lines = 0; $lines <= 1; $lines++){echo $users[$lines][0] . ' ' . $users[$lines][1] . '<br />';}
	// 20 Dexter74
	// 21 Drthrax74
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
#### 1. Complex
```php

<?php
	// Déclaration du tableau (Non numérotés)
	$BDD = [
  	       ['20','Dexter74','Passw0rd2022','Jaques','Levin','31','dexter74@mail.com','users'],
  	       ['21','Drthrax74','Passw0rd2022','Paul','Courrier','31','drthrax74@mail.com','Administrateur'],
  	       ['22','Snake','Passw0rd2022','Alain','Charles','31','drthrax74@mail.com','Administrateur'],
  	       ];
	// Lecture des lignes 0 et 1. Coloone 1 et 6.
	for ($LIGNE = 0; $LIGNE <=1; $LIGNE++){echo $BDD[$LIGNE][1] .'('.	$BDD[$LIGNE][6] .')'. '<br />';}
?>
```



ERREUR
```php
<?php
	// Déclaration du tableau (Non numérotés)
	$BDD = [
  	       ['20','Dexter74','Passw0rd2022','Jaques','Levin','31','dexter74@mail.com','users'],
  	       ['21','Drthrax74','Passw0rd2022','Paul','Courrier','31','drthrax74@mail.com','Administrateur'],
  	       ['22','Snake','Passw0rd2022','Alain','Charles','31','drthrax74@mail.com','Administrateur'],
  	       ];
	// Lecture de la ligne 0 à 1 du tableau
	for ($LIGNE = 0; $BDD <= 1; $BDD++){echo "Utilisateur: '. $BDD[$LIGNE][2] .' ('. $BDD[$LIGNE][7] .')"}
?>
```



<br />

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
| 2  | Franck      |
| 3  | Marc        |

###### Construire un Tableau Numéroté
```php
<?php
	// Déclaration d'un Tableau (Non numérotés)
	$VALEUR0 = ['Jean-Claude', 'Halidi', 'Franck', 'Marc'];
	// Déclaration d'un tableau indexé numériquement
	$VALEUR1 = array('Jean-Claude', 'Halidi', 'Franck', 'Marc');
?>
```

<br />

--------------------------------------------------------
### B. Familiarisez-vous avec les tableaux associatifs
#### 1. Construisez un tableau associatif (2 Manières d'écritures)
```php
<?php
	$TABLEAU = 	[
		'TITRE' => 'Independance Day ',
		'JOUR'	=> '2 ',
		'MOIS'	=> 'Octobre ',
		'ANNEE'	=> '1996 ',
		];
?>
```

```php
<?php
	$TABLEAU['TITRE'] = 'Independance Day';
	$TABLEAU['JOUR'] = '2';
	$TABLEAU['MOIS'] = 'Octobre';
	$TABLEAU['ANNEE'] = '1996';
?>
```

#### 2. Affichez un tableau associatif
```php
<?php
	echo $TABLEAU['TITRE'];
?>
```

#### 3. Quand utiliser un tableau numéroté et quand utiliser un tableau associatif ?
```
Les tableaux numérotés:
	- Permettent de stocker une série d'éléments du même type, comme des prénoms.
	- Chaque élément du tableau contiendra alors un prénom.
	
Les tableaux associatifs:
	- Permettent de découper une donnée en plusieurs sous-éléments. 
	- Par exemple, une adresse peut être découpée en nom, prénom, nom de rue, ville…
```

<br />

--------------------------------------------------------
### C. Parcourez un tableau
#### 1. La boucle for
```php
<?php
	$TABLEAU = [
		['Independance Day I', '2', 'Octobre', '1996',],
		['Independance Day II', '20', 'Juillet', '2016',],
		['Armageddon', '5', 'août ', '1998',],
		];
	
	// Independance Day IIndependance Day II
	for ($Ligne = 0; $Ligne <= 1; $Ligne++) {echo $TABLEAU[$Ligne][0];}
?>
```
#### 2. La boucle foreach 
```php
<?php
	$TABLEAU = [
		['Independance Day I ', '2', 'Octobre', '1996',],
		['Independance Day II', '20', 'Juillet', '2016',],
		['Armageddon', '5', 'août ', '1998',],
		];
	
	// Independance Day I Independance Day IIArmageddon
	foreach ($TABLEAU as $RESULTAT ) {echo $RESULTAT[0];}
?>
```

```php
<?php
	$TABLEAU = [
		'TITRE' => 'Independance Day -',
		'JOUR'	=> '2 ',
		'MOIS'	=> 'Octobre ',
		'ANNEE'	=> '1996 ',
		];
	
	// Independance Day -2 Octobre 1996
	foreach ($TABLEAU as $RESULTAT) {echo $RESULTAT;}
?>
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
#### 1. Les types de recherches
```php
array_key_exists : Pour vérifier si une clé existe dans le tableau.
in_array	 : Pour vérifier si une valeur existe dans le tableau.

array_search 	 : Pour récupérer la clé d'une valeur dans le tableau.
```

#### 2. Vérifiez si une clé existe dans un tableau
```php
<?php

$TABLEAU = [
	'user1' => 'Marc',
	'user2' => 'Franck',
	'user3' => 'Philippe',
	'user4' => 'Isabelle',
	];

if (array_key_exists('user1', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user1'] . ' existe';
	echo '<br />';

if (array_key_exists('user2', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user2'] . ' existe';
	echo '<br />';

if (array_key_exists('user3', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user3'] . ' existe';
	echo '<br />';

if (array_key_exists('user4', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user4'] . ' existe';
	echo '<br />';


if (array_key_exists('user5', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user5'] . ' existe';
	echo '<br />';

?>
```

#### 3. Vérifiez si une valeur existe dans un tableau
```php
<?php

$TABLEAU = [
	'user1' => 'Marc',
	'user2' => 'Franck',
	'user3' => 'Philippe',
	'user4' => 'Isabelle',
	];

if (in_array('Marc', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user1'] . ' existe';
	echo '<br />';

if (in_array('Franck', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user2'] . ' existe';
	echo '<br />';

if (in_array('Philippe', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user3'] . ' existe';
	echo '<br />';

if (in_array('Isabelle', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user4'] . ' existe';
	echo '<br />';


if (array_key_exists('user5', $TABLEAU))
	echo 'L\'utilisateur ' . $TABLEAU['user5'] . ' existe';
	echo '<br />';
?>
```


#### 4. Récupérez la clé d'une valeur dans un tableau
```php
<?php
	// Déclaration d'un Tableau (Non numérotés)
	$USERS    = [ 'Marc', 'Franck' , 'Philippe', 'Isabelle' ];
	
	// Rechercher le numéro de l'utilisateur
	$MARC = array_search('Marc',$USERS);
	$FRANCK = array_search('Franck',$USERS);
	$PHILIPPE = array_search('Philippe',$USERS);
	$ISABELLE = array_search('Isabelle',$USERS);

echo '<b>MARC est en position</b> ' . $MARC;
echo '<br />';
echo '<b>FRANCK est en position</b> ' . $FRANCK;
echo '<br />';
echo '<b>PHILIPPE est en position</b> ' . $PHILIPPE;
echo '<br />';
echo '<b>ISABELLE est en position</b> ' . $ISABELLE;
?>
```

<br />


--------------------------------------------------------
### E. Affichez des recettes (version 2 !)
#### 
#### 2. 
```php
<?php
// Déclaration du Tableau des News
$TABLEAU = 	[
		[
			'Visible'	=> true,
			'title' 	=> 'Titre 1',
			'article'	=> 'Contenu de mon article 1',
			'auteur'	=> 'Marc',
			'date'		=> '21/10/22',
			'heure'		=> '02:39',
		],	

		[
			'Visible'	=> true,
			'title' 	=> 'Titre 2',
			'article'	=> 'Contenu de mon article 2',
			'auteur'	=> 'Franck',
			'date'		=> '21/10/22',
			'heure'		=> '02:46',
		],	
							
];
?>

<!DOCTYPE html>
<html>
	<head>
		<title>Affichage des recettes</title>
	</head>
	<body>
		<h1>Affichage des recettes</h1>
			<!-- Boucle sur les recettes -->
			<?php foreach($TABLEAU as $RESULT) : ?>
				<!-- si la clé existe et a pour valeur "vrai", on affiche -->
				<?php if (array_key_exists('Visible', $RESULT) && $RESULT['Visible'] == true ): ?>
					<article>
						<h3><?php echo $RESULT['title']; ?></h3>
						<div><?php echo $RESULT['article']; ?> </div>
						<div><?php echo 'Posté Par '.'<b>'.$RESULT['auteur'].'</b>'.' le '.'<b>'.$RESULT['date'].'</b>'.' à '.'<b>'.$RESULT['heure'].'</b>'; ?></div>
						
						<?php echo '<br />'; ?> 
					</article>
				<?php endif; ?>
		<?php endforeach ?>
	</body>
</html>

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
