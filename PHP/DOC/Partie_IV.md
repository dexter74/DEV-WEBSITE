-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Ecrire ses propres fonctions](http://formation.upyupy.fr/php-mysql/ecrire-fonction-php/)</p>

### A. Les fonctions
#### 1. Définir une fonction
```php
<!-- Fonction sans paramètre --> 
<?php
  function maFonctionA() {echo "Fonction A";}
?>

<!-- Fonction avec paramètre --> 
<?php 
  function maFonctionB($parametre) {echo "Fonction B";} 
?>

<?php
  function maFonctionC($a, $b, $c) {echo "Fonction C";}
?>
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
