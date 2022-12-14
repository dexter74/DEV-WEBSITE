---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Mettez en place le CSS](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605060-mettez-en-place-le-css)</p>

#### A. Où écrit-on le CSS ?
```html
<head>
  <link rel="stylesheet" href="style.css" />
<head>
```

#### B. Appliquer un style : sélectionner une balise
###### HTML et CSS
```
<h1>Test </h1>
<p>Salut à tous.</p> 

p, h1 { color: blue; }
```

#### C. Appliquer un style : class et id
```
id:  :  Utilisable une seule Fois. (CSS: #)
class:  Utilisable infinie (CSS: .) 
```

###### HTML et CSS
```
<div clss="TEST1"></div>
<div id="TEST2"></div>

.TEST1 { }
#TEST2 { }
```

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Formatez du texte](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605329-formatez-du-texte) </p> 

#### A. La taille
###### 1. La taille absolue
```css
font-size: 16px;
```
###### 2. Une valeur relative
```css
font-size: xx-small; /* Minuscule   */
font-size: x-small;  /* Très petit  */
font-size: small;    /* Petit       */
font-size: medium;   /* Moyen       */
font-size: large;    /* Grand       */
font-size: x-large;  /* Très grand  */
font-size: xx-large; /* Gigantesque */
```

#### B. La police
###### 1. Général
```css
font-family: Verdana,arial;
```
###### 2.a Police Personnalisée [Convertir TTF](https://www.fontsquirrel.com/tools/webfont-generator)
```css
@font-face {
  font-family: 'MaSuperPolice';
  src: url('MaSuperPolice.eot')  format('eot'),
       url('MaSuperPolice.woff') format('woff'),
       url('MaSuperPolice.ttf')  format('truetype'),
       url('MaSuperPolice.svg')  format('svg');
}
```

###### 2.b Police Google
```
Aller sur https://fonts.google.com/
Choisir la police, aller dans la section Style.
Cliquer sur le bouton "Thin XXX"
Copier le code "<link> ou @import" dans la balise header.
Mettre mon style.css en dessous.
Dans le style.css coller le code "CSS rules to specify families" dans la balise souhaitée.
```


###### 3. Italique
```css
font-style: normal;
font-style: oblique;
font-style: italic;
```
###### 4. Gras
```css
font-weight: bold;
```
###### 5. Souligné
```css
text-decoration: none;         /* Aucun soulignement	*/
text-decoration: underline;    /* Souligné        	*/

text-decoration: line-through; /* Barré           	*/
text-decoration: overline;     /* Ligne au-dessus 	*/ 
```
###### 6. L'alignement
```css
text-align: left;     /* Aligner le texte à Gauche    */
text-align: right;    /* Aligner le texte à Droite    */
text-align: center;   /* Aligner le texte à Centre    */
text-align: justify;  /* Aligner le texte à Justifier */
```

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'>[Ajoutez de la couleur et un fond](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605551-ajoutez-de-la-couleur-et-un-fond) </p>

#### A. Couleur du texte ([ColorPicker](http://www.colorpicker.com/))
```css
color: maroon;
color: #FFFFFF;
color: rgb(240,96,204);
```

#### B. Couleur de fond
```css
background-color: black;
```

#### C.Images de fond
###### 1. Appliquer une image de fond
```css
background-image: url("");      /* Image de Fond  */
background-size: 100%;          /* Etirer le fond */    
```
###### 2. Options disponibles pour l'image de fond
```css
/* Fixer le fond */
background-attachment: fixed;     /* Le fond est fixe */
background-attachment: scroll;    /* Le fond défile   */

/* Répétition du fond */
background-repeat: no-repeat;     /* Le fond ne sera pas répété. L'image sera donc unique sur la page      */
background-repeat: repeat-x;      /* Le fond sera répété uniquement sur la première ligne, horizontalement */
background-repeat: repeat-y;      /* Le fond sera répété uniquement sur la première colonne, verticalement */
background-repeat: repeat;        /* Le fond sera répété en mosaïque (par défaut)                          */

/* Position du fond */
background-position: no-repeat;   /* Le fond ne se répéte pas */
background-position: XXpx XXpx;   /* Gauche, Haut             */
background-position: top;         /* En haut                  */
background-position: bottom;      /* En bas                   */
background-position: left;        /* A Gauche                 */
background-position: center;      /* Au Centre                */
background-position: right;       /* A droite                 */
background-position: top right;   /* Aligner en Haut à droit  */

/* Combiner les Propriétés */
background: url("soleil.png") fixed no-repeat top right;  /* Fond Fixe + Ne se répète pas +  Haut + droite


/* Exemple */
	background-image: url(/image/background.jpg);
	background-attachment: fixed;
	background-size: 100% 100%;
```

#### D.La transparence
```css
opacity: 0.6; /* 60% */
```

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'>[Créez des bordures et des ombres](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605694-creez-des-bordures-et-des-ombres) </p>

#### A. Bordures standard
###### 1. Les Bordures
```css
border: <largeur px> <Couleur> <Type>;
                               none;    /* Pas de bordure */
                               solid;   /* Trait Simple */
                               dotted;  /* Pointillés */
                               dashed;  /* Tiret */
                               double;  /* Bordure Double */
                               groove;  /* Relief */
                               ridge;   /* Autre effet de relief */
                               inset;   /* Effet 3D Global enfoncé */
                               outset;  /* effet 3D Global surélevé */
border: 2px black solid; 
```
###### 2. Définir un côté d'une bordure
```css
border-top: 1px;    /* Bordure du haut    */
border-bottom: 1px; /* Bordure du bas     */
border-left: 1px;   /* Bordure de gauche  */
border-right: 1px;  /* Bordure de droite  */

border-right: 3px black solid;
```

#### B. Bordures arrondies
```css
border-radius: <Haut Gauche> <Haut Droit> <Bas Droit> <Bas Gauche>;
border-radius: 0px 0px 15px 15px;
```

#### C. Les ombres
###### 1. Les ombres des boîtes
```css
box-shadow: <Le décalage horizontal de l'ombre> <Le décalage vertical de l'ombre> <L'adoucissement du dégradé> <La couleur de l'ombre>

box-shadow: 0px 0px 0px red inset;
box-shadow: 0px 0px 0px red;
```

###### 2. L'ombre du texte
```css
text-shadow: 0px 0px 0px black; 
```

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Créez des apparences dynamiques](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605763-creez-des-apparences-dynamiques) </p>

#### A. Au survol
```css
a /* Liens par défaut (non survolés) */
{
   text-decoration: none;
   color: red;
   font-style: italic;
}

a:hover /* Apparence au survol des liens */
{
   text-decoration: underline;
   color: green;
}
```
#### B. Au clic et lors de la sélection
###### 1. Au moment du clic
```css
a:active /* Quand le visiteur clique sur le lien */
{
    background-color: #FFCC66;
}
```
###### 2. Lorsque l'élément est sélectionné
```css
a:focus /* Quand le visiteur sélectionne le lien */
{
    background-color: #FFCC66;
}
```
#### C. Lorsque le lien a déjà été consulté
 ```css
 a:visited /* Quand le visiteur a déjà vu la page concernée */
{
    color: #AAA; /* Appliquer une couleur grise */
}
```
