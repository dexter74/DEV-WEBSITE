---------------------------------------------------------------------------------------------------------------------------------------------------------------
## I. [Mettez en place le CSS](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605060-mettez-en-place-le-css)
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
class: Utiliser un . devant le nom. Utilisable une seule Fois.
id:  : Utiliser un # devant le nom. Objet Unique.
```

###### HTML et CSS
```
<div clss="TEST1"></div>
<div id="TEST2"></div>

.TEST1 { }
#TEST2 { }
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------
## II. [Formatez du texte](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605329-formatez-du-texte)
#### A. La taille
###### 1. La taille absolue
```css
font-size: 16px;
```
###### 2. Une valeur relative
```css
font-size: xx-small; /* minuscule   */
font-size: x-small;  /* très petit  */
font-size: small;    /* petit       */
font-size: medium;   /* moyen       */
font-size: large;    /* grand       */
font-size: x-large;  /* très grand  */
font-size: xx-large; /* Gigantesque */
```

#### B. La police
###### 1. Général
```css
font-family: Verdana,arial;
```
###### 2. Police Personnalisée
```css
@font-face {
  font-family: 'MaSuperPolice';
  src: url('MaSuperPolice.eot')  format('eot'),
       url('MaSuperPolice.woff') format('woff'),
       url('MaSuperPolice.ttf')  format('truetype'),
       url('MaSuperPolice.svg')  format('svg');
}
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
text-decoration: underline;    /* Souligné        */
text-decoration: line-through; /* barré           */
text-decoration: overline;     /* Ligne au-dessus */ 
text-decoration: none;         /* Normal (Défaut) */
```

###### 6. L'alignement
```css
text-align: left;     /* Aligner le texte à Gauche    */
text-align: right;    /* Aligner le texte à Droite    */
text-align: center;   /* Aligner le texte à Centre    */
text-align: justify;  /* Aligner le texte à Justifier */
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------
## III. [Ajoutez de la couleur et un fond](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605551-ajoutez-de-la-couleur-et-un-fond)

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
background-image: url("");      /* Image de Fond */
```
###### 2. Options disponibles pour l'image de fond
```css
/* Fixer le fond */
background-attachment: fixed;   /* Le fond est fixe */
background-attachment: scroll;  /* Le fond défile   */

/* Répétition du fond */
background-repeat: no-repeat;   /* Le fond ne sera pas répété. L'image sera donc unique sur la page      */
background-repeat: repeat-x;    /* Le fond sera répété uniquement sur la première ligne, horizontalement */
background-repeat: repeat-y;    /* Le fond sera répété uniquement sur la première colonne, verticalement */
background-repeat: repeat;      /* Le fond sera répété en mosaïque (par défaut)                          */

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

```

#### D.La transparence
```css
opacity: 0.6; /* 60% */
```


---------------------------------------------------------------------------------------------------------------------------------------------------------------
## IV. [Créez des bordures et des ombres](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605694-creez-des-bordures-et-des-ombres)
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

border: 5px blue 
```
###### 2.
###### 3.
###### 4.
#### B. Bordures arrondies
#### C. Les ombres



