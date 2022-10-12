------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Écrivez votre premier script](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/4238116-ecrivez-votre-premier-script)</p>

#### A Utilisez des balises PHP
###### 1. Page HTML de Base
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Ma page web</title>
    </head>
    
    <body>
        <h1>Ma page web</h1>
        <p>
            Bonjour <!-- Insérer le pseudo du visiteur ici --> !
        </p>

    </body>
</html>
```
###### 2. Reconnaissez la forme d'une balise PHP
```php
<?php
.....
?>
```

###### 3. Insérez une balise PHP au milieu du code HTML
```php
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Ma page web</title>
    </head>
    
    <body>
        <h1>Ma page web</h1>
        <p>
            Bonjour <!-- Insérer le pseudo du visiteur ici --> !
        </p>
        <!-- ###################### -->        
        <?php
        /* Encore du PHP
        Toujours du PHP */
        ?>
        <!-- ###################### -->        
    </body>
</html>
```

#### B Affichez du texte
###### 1. Instrcution echo (2 méthodes)
```php
<?php echo "Ceci est du texte"; ?>
ou
<?php echo("Ceci est du texte"); ?>
```
###### Exemple
```php
<?php echo "Ceci est du <strong>texte</strong>"; ?>
<?php echo "Cette ligne a été écrite \"uniquement\" en PHP."; ?>
```

#### C Commentez votre code
###### 1. Mono-Ligne
```php
<?php
    echo "J'habite en Chine."; // Cette ligne indique où j'habite
    // La ligne suivante indique mon âge
    echo "J'ai 92 ans.";
?>
```

###### 1. Multi-Lignes
```php
<?php
    /* Début de Mon commentaire
       Fin de commentaire */
    echo "J'ai 92 ans.";
?>
```



------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Configurez PHP pour visualiser les erreurs](https://openclassrooms.com/fr/courses/918836-concevez-votre-site-web-avec-php-et-mysql/4238821-configurez-php-pour-visualiser-les-erreurs)</p>


#### A Configurez PHP pour afficher les erreurs
###### 1. Localisez le fichier de configuration PHP du serveur web
```php
<?php
phpinfo();
```
###### Exemple
```
Loaded Configuration File	/usr/local/AppCentral/php7/etc/php.ini
```

###### 2. Modifiez le fichier de configuration PHP
Il faut s'assurer des valeurs suivantes
```php
error_reporting = E_ALL
display_errors = On
```

**Check**
```console
grep "display_errors" /usr/local/AppCentral/php7/etc/php.ini
```

**Backup**
```console
cp  /usr/local/AppCentral/php7/etc/php.ini /usr/local/AppCentral/php7/etc/php.ini.old
chattr +i  /usr/local/AppCentral/php7/etc/php.ini.old
```

**Edittion**
```console
chattr -i /usr/local/AppCentral/php7/etc/php.ini
sed -i -e 's/display_errors \= Off/display_errors \= On/' /usr/local/AppCentral/php7/etc/php.ini

#Relancer le service Web
```

#### B Testez l'affichage des erreurs
```php
<?php
phpinfo(;
```
