------------------------------------------------------------------------------------------------------------------------------------------

### [Créez votre première page web en HTML](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604361-creez-votre-premiere-page-web-en-html)

#### Les balises et leurs attributs
**Les balises en paires**
````html
<titre>Ceci est un titre</titre>
Ceci n'est pas un titre <titre>Ceci est un titre</titre> Ceci n'est pas un titre
````
**Les balises orphelines**
````html
<image />
````
**Les Attributs**
````html
<balise attribut="valeur">
<image nom="photo.jpg" />
  
<citation auteur="Neil Armstrong" date="21/07/1969">
C'est un petit pas pour l'homme, mais un bond de géant pour l'humanité.
</citation>
````
#### Structure de base d'une page HTML5
````html
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
````
**Le doctype**
````html
<!DOCTYPE html>
````
**La balise </html>**
````html
<html>
 ..
</html>
````
**L'en-tête**
````html
<head>
 ..
</head>
````
**Le Corps**
````html
<body>
 ..
</body>
````
**L'encodage**
````html
<meta charset="utf-8" />
````
**Le titre principal de la page**
````html
<title>Marc</title>
````
#### Les commentaires
````html
<!-- Ceci est un commentaire -->
````

------------------------------------------------------------------------------------------------------------------------------------------
### [Organisez votre texte](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604534-organisez-votre-texte)

#### Les paragraphes
````html
<p>Bonjour et bienvenue sur mon site !</p>
````
**Sauter une ligne**
````html
<br />
````
#### Les titres
````html
<h1> </h1>  : signifie « titre très important ». En général, on s'en sert pour afficher le titre de la page au début de celle-ci ;
<h2> </h2>  : signifie « titre important » ;
<h3> </h3>  : pareil, c'est un titre un peu moins important (on peut dire un « sous-titre », si vous voulez) ;
<h4> </h4>  : titre encore moins important ;
<h5> </h5>  : titre pas important ;
<h6> </h6>  : titre vraiment, mais alors là vraiment pas important du tout.
````
#### La Mise en Valeur
**Italic**
````html
<em> </em>
````
**important**
````html
<strong> </strong>
````
**Marquer le texte**
````html
<mark> </mark>
````
#### Les Listes
````
ul: délimite toute la liste
li: délimite un élément de la liste.
````

**Création d'une liste**
````html
<ul> </ul>
<ol> </ol>
````
**Élément de la liste**
````html
<li>Mon Menu</li>
````
**Liste Non-ordonnée**
````html
<ul>
 <li>Mon Menu</li>
</ul>
````
**Liste ordonnée**
````html
<ol>
 <li>Mon Menu</li>
</ol>
````

------------------------------------------------------------------------------------------------------------------------------------------
### [Créez des liens](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604646-creez-des-liens)
#### Un lien vers un autre site
````html
<a href="#">Menu</a>
````
#### Un lien vers une ancre
**Création d'une Ancre**
````html
<h2 id="mon_ancre">Titre</h2>
````
**Liens pointant vers l'ancre**
````html
<a href="#mon_ancre">Aller vers l'ancre</a>
````

**Divers**
````html
<p>Bonjour. Souhaitez-vous visiter <a href="https://openclassrooms.com" title="Vous ne le regretterez pas !">OpenClassrooms</a> ?</p>
````
````html
<p>Bonjour. Souhaitez-vous visiter <a href="https://openclassrooms.com" title="Vous ne le regretterez pas !" target="_blank">OpenClassrooms</a> ?</p>
````
````html
<p><a href="mailto:votrenom@bidule.com">Envoyez-moi un e-mail !</a></p>
````
````html
<p><a href="monfichier.zip">Télécharger le fichier</a></p>
````


------------------------------------------------------------------------------------------------------------------------------------------
### [Insérez des images](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1604791-inserez-des-images)

#### Insérer une image
````html
<img src="" alt="" title="" />
````
#### Miniature Cliquable
````html
<a href="img/pleinformat.jpg"><img src="img/miniformat.jpg" alt="" title="" /></a>
````
#### Les figures ===> ???
````html
````
