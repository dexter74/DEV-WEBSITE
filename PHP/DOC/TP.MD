-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> Tous les TP sont justes </p>
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## A. Décrivez les éléments de votre projet à l'aide de variables

### 1. Affectez une valeur à une variable / Affichez le contenu d'une variable
```php
<?php
  // ---------------------------------------------------
	$fullname = "Mathieu Nebra";
	$email = 'mathieu.nebra@exemple.com';
	$prenom1 = "Mon \"nom\" est Mathieu";
	$prenom2 = 'Je m\'appelle Mathieu';
	$userAge = 17;
	$price = 57.3;
	$isAuthor = true;
	$isAdministrator = false;
	$noValue = NULL;
// ---------------------------------------------------
	echo "<b> Afficher le résultat en mode collé: </b>";
	echo $email;
	echo $fullname;
	echo $prenom1;
	echo $prenom2;
	echo $isAuthor;
	echo $userAge;
	echo $price;
	echo $noValue;
	echo "<br />";
	echo "<br />";
	echo "<b> Afficher résultat sur une ligne en mode Propre: </b>";
	echo $email . ' | ' . $fullname . ' | ' . $prenom1 . ' | ' . $prenom2	. ' | ' .	$isAuthor . ' | ' .	$userAge . ' | ' . $price . ' | ' . $noValue;
	echo "<br />";
	echo "<br />";
	echo "<b> Afficher le résultat sur plusieurs ligne: </b>";
	echo "<br />";
	echo $email		. '<br />';
	echo $fullname . '<br />';
	echo $prenom1	. '<br />';
	echo $prenom2	. '<br />';
	echo $isAuthor . '<br />';
	echo $userAge	. '<br />';
	echo $price		. '<br />';
	echo $noValue	. '<br />';
?>
```


### 2. Concaténez une variable
```php
<?php
	$NOMINATION = 'Marc Jaffré';
	echo 'Bonjour ';
	echo $NOMINATION;
	echo ' et bienvenue sur mon site.';
?>
```

### 3. Calculs Simples
```php
<?php
	$ANNEE      = '2022';
	$NAISSANCE  = '1980';
	$AGE        =($ANNEE - $NAISSANCE); 
	$CENTENAIRE =($NAISSANCE + 100); 
	echo '<b> Calcul ton age: </b>' . $ANNEE . ' - ' . $NAISSANCE . ' = ' . $AGE . ' ans';
?>
```

<br />


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## B. Appropriez-vous la structure de base : if… else

### SI, SINON, SINON SI
```php
<?php
	$TEST1 = '0';
	$TEST2 = '1';
	$TEST3 = '2';
	$OK    = '✅';
	$KO    = '❌';
	$ABEND = '???';

// ------------------------------------------------------------------------------
	echo "<b>Exercice 1: SI: </b>";
	if($TEST1 == 0){echo $OK;}
	echo '<br />';
// ------------------------------------------------------------------------------
	echo "<b>Exercice 2: SI + SINON: </b>";
	if($TEST2 == 0){echo $OK;}
	else{echo $KO;}
	echo '<br />';
// ------------------------------------------------------------------------------
	echo "<b>Exercice 3: Si + SINON + SINON SI: </b>";
	if($TEST3 == 0){echo $OK;}
	elseif($TEST3 == 1){echo $KO;}
	else{echo $ABEND;}
	echo '<br />';
// ------------------------------------------------------------------------------
	echo "<b>Exercice 4: AND: </b>";
	if($TEST1 == '0' && $TEST2 = '1' && $TEST3 == '3' ){echo $OK;}
	else{echo $KO;}
	echo '<br />';
// ------------------------------------------------------------------------------
//	echo "<b>Exercice 5: OR: </b>";
?>
```





-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## C.
```php
<?php
	// Tableau (Non numéroté)
	$user0 = ['20','Dexter74','Passw0rd2022','Jaques','levin','31','dexter74@mail.com','users'];
	$user1 = ['21','Drthrax74','Passw0rd2022','Paul','courrier','31','drthrax74@mail.com','Administrateur'];

	// Tableau dans un Tableau
	$users = [$user0, $user1];
	
	// Code de Sortie sur la page PHP
	echo '<b>Interroger dans un tableau:</b>';
	echo '<br />';
	echo '<b>- ID: </b>' . $user0[0];
	echo '<br />';
	echo '<b>- USERNAME: </b>' . $user0[1];
	echo '<br />';
	echo '<b>- Email: </b>' . $user0[6];
	
	// Retour de page
	echo '<br />';
	
	// Saut de page
	echo '<br />';
	
	echo '<b>Interroger dans un tableau dans un tableau:</b>';
	echo '<br />';
	echo '<b>- ID: </b>' . $users[0][0];
	echo '<br />';
	echo '<b>- USERNAME: </b>' . $users[0][1];
	echo '<br />';
	echo '<b>- Email: </b>' . $users[0][6];
?>
```


