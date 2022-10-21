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

### B. Réaliser un calcul
```php

<!-- Déclaration de la fonction avec paramètres (x, y, z) -->
<?php function calcul($x, $y, $z) {$result=($x-$y)/$z; echo $result;} ?>

<!-- Appeler la fonction avec 3 arguments (x, y, z) -->
<?php calcul(100, 5, 5); ?>
```
