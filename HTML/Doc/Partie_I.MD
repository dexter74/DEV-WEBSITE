------------------------------------------------------------------------------------------------------------------------------------------

### <p align='center'> [Créez votre première page web en HTML](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604361-creez-votre-premiere-page-web-en-html) </p>

#### A Les balises et leurs attributs
###### 1. Les balises en paires
```html
<titre>Ceci est un titre</titre>
Ceci n'est pas un titre <titre>Ceci est un titre</titre> Ceci n'est pas un titre
```
###### 2. Les balises orphelines
```html
<image />
```
###### 3. Les Attributs
```html
<balise attribut="valeur">
<image nom="photo.jpg" />
<citation auteur="Neil Armstrong" date="21/07/1969">
C'est un petit pas pour l'homme, mais un bond de géant pour l'humanité.
</citation>
```
#### B. Structure de base d'une page HTML5

##### 1. HTML
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Titre</title>
        <link rel="stylesheet" href="style.css" />
    </head>
    <body>
    </body>
</html>
```
##### 2. CSS
```css
body{ margin:  0px;}
body{ padding: 0px;}
```

###### 1. Le doctype
```html
<!DOCTYPE html>
```

###### 2. La balise </html>
```html
<html></html>
```

###### 3. L'en-tête
```html
<head></head>
```
###### 4. Le Corps
```html
<body></body>
```
###### 5. L'encodage
```html
<meta charset="utf-8" />
```
###### 5. Le titre principal de la page
```html
<title></title>
```
#### C. Les commentaires
```html
<!-- Ceci est un commentaire -->
```

<br />

------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'>[Organisez votre texte](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604534-organisez-votre-texte) </p>

#### A. Les paragraphes
```html
<p>Bonjour et bienvenue sur mon site !</p>
```
###### 1. Sauter une ligne
```html
<br />
```

#### B. Les titres
```html
<h1> </h1>  : signifie « titre très important ». En général, on s'en sert pour afficher le titre de la page au début de celle-ci ;
<h2> </h2>  : signifie « titre important » ;
<h3> </h3>  : pareil, c'est un titre un peu moins important (on peut dire un « sous-titre », si vous voulez) ;
<h4> </h4>  : titre encore moins important ;
<h5> </h5>  : titre pas important ;
<h6> </h6>  : titre vraiment, mais alors là vraiment pas important du tout.
```

#### C. La Mise en Valeur
###### 1. Italic
```html
<em> </em>
```
###### 2. important
```html
<strong> </strong>
```
###### 3. Marquer le texte
```html
<mark> </mark>
```
###### C. Les Listes
```
ul: délimite toute la liste
li: délimite un élément de la liste.
```
###### 1. Création d'une liste
```html
<ul> </ul>
<ol> </ol>
```
###### 2. Élément de la liste
```html
<li>Mon Menu</li>
```
###### 3. Liste Non-ordonnée
```html
<ul>
 <li>Mon Menu</li>
</ul>
```
###### 4. Liste ordonnée
```html
<ol>
 <li>Mon Menu</li>
</ol>
```

<br />

------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Créez des liens](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604646-creez-des-liens) </p>
#### A. Un lien vers un autre site
```html
<a href="https://openclassrooms.com">OpenClassrooms</a>
```

#### B. Un lien vers une autre page de son site
```html
<p>Bonjour. Souhaitez-vous consulter <a href="page2.html">la page 2</a> ?</p>
<a href="contenu/page2.html">
<a href="../page2.html">
```

#### C. Un lien vers une ancre
###### 1. Création d'une Ancre
```html
<h2 id="mon_ancre">Titre</h2>
```
###### 2. Liens pointant vers l'ancre**
```html
<a href="#mon_ancre">Aller vers l'ancre</a>
```

#### D. Cas pratiques d'utilisation des liens
###### 1. Divers
```html
<p>Bonjour. Souhaitez-vous visiter <a href="https://openclassrooms.com" title="Vous ne le regretterez pas !">OpenClassrooms</a> ?</p>
```
```html
<p>Bonjour. Souhaitez-vous visiter <a href="https://openclassrooms.com" title="Vous ne le regretterez pas !" target="_blank">OpenClassrooms</a> ?</p>
```
```html
<p><a href="mailto:votrenom@bidule.com">Envoyez-moi un e-mail !</a></p>
```
```html
<p><a href="monfichier.zip">Télécharger le fichier</a></p>
```


------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'>[Insérez des images](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604791-inserez-des-images) </p>

#### A. Insérer une image
```html
<img src="" alt="" title="" />
```
###### 1. Miniature Cliquable
```html
<a href="img/pleinformat.jpg"><img src="img/miniformat.jpg" alt="" title="" /></a>
```



#### B. Les figures ===> ???
```html
```
