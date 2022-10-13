
#### Tableau:

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

```
<?php
Tableau des correspondances
$user0 = ['20','Dexter74','Passw0rd2022','Jaques','levin','31','dexter74@mail.com','users'];
$user1 = ['21','Drthrax74','Passw0rd2022','Paul','courrier','31','drthrax74@mail.com','Administrateur'];

Tableau regroupant les correspondances
$users = [$user0, $user1];

Interroger dans un tableau
	echo '<b>Information:</b>';
	echo '<br />';
	echo '<b>- ID: </b>' . $user0[0];
	echo '<br />';
	echo '<b>- USERNAME: </b>' . $user0[1];
	echo '<br />';
	echo '<b>- Email: </b>' . $user0[6];


 Interroger dans un tableau dans un tableau
	echo '<b>Information:</b>';
	echo '<br />';
	echo '<b>- ID: </b>' . $users[0][0];
	echo '<br />';
	echo '<b>- USERNAME: </b>' . $users[0][1];
	echo '<br />';
	echo '<b>- Email: </b>' . $users[0][6];

?>
```
