-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Ecrire ses propres fonctions](http://formation.upyupy.fr/php-mysql/ecrire-fonction-php/)</p>

### A. Les fonctions
#### 1. Définir une fonction
```php
	<!-- Fonction A sans paramètre --> 
	<?php function maFonctionA() {echo "Fonction A";} ?>
  
	<!-- Fonction B avec 1 paramètre --> 
	<?php function maFonctionB($parametre) {echo $parametre;} ?>

	<!-- Fonction C avec 3 paramètres --> 
	<?php function maFonctionC($a, $b, $c) {echo $a, $b, $c;} ?>
```

#### 2. Appeler une fonction
```php
	<!-- Appeler la fonction A -->
	<?php maFonctionA(); ?>
	<br />

	<!-- Appeler la fonction B -->
	<?php maFonctionB("voiture"); ?>
	<br />

	<!-- Appeler la fonction C -->
	<?php maFonctionC(12, 25, 1); ?>
```

#### 3. Réaliser un calcul
```php
<?php 
	// Déclaration de la fonction avec paramètres (x, y, z)
	function calcul($x, $y, $z)
	{
	$result=($x-$y)/$z;
	echo $result. " %";
	}
?>
<?php 
	// Appeler la fonction avec 3 arguments (x, y, z) -->
	calcul(100, 5, 5);
?>
```

#### 4. Permettre à une fonction de retourner une valeur.
```php
<?php
	// Déclaration de la fonction avec paramètres (x, y, z)
	function calcul($x, $y, $z)
	{
	$result=($x-$y)/$z;
	return $result. " %";
	}
	
	// Permettre à une fonction de retourner une valeur (x, y, z)
	$VAR = calcul(100, 5, 5) 
?>

<?php
	// Appeler la fonction avec 3 arguments (x, y, z)
	echo $VAR 
?>
```
