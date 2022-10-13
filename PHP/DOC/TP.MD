-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### A. Affectez une valeur à une variable
```php
<?php
  $fullname = "Mathieu Nebra";
  $email = 'mathieu.nebra@exemple.com';
  $prenom1 = "Mon \"nom\" est Mathieu";
  $prenom2 = 'Je m\'appelle Mathieu';
  $userAge = 17;
  $price = 57.3;
  $isAuthor = true;
  $isAdministrator = false;
  $noValue = NULL;
  
  echo $email    . '<br />';
  echo $fullname . '<br />';
  echo $prenom1  . '<br />';
  echo $prenom2  . '<br />';
  echo $isAuthor . '<br />';
  echo $userAge  . '<br />';
  echo $price    . '<br />';
  echo $noValue  . '<br />';
?>
```

<br />

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### Tableau (Non numéroté)
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
	echo '<br />';
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


