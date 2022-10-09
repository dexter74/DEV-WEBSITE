------------------------------------------------------------------------------------------------------------------------------------------
### [Mettez en place le CSS](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605060-mettez-en-place-le-css)
#### Où écrit-on le CSS ?
```html
<head>
  <link rel="stylesheet" href="style.css" />
<head>
```
#### Appliquer un style : sélectionner une balise
**Code HTML**
```html
<h1>Test </h1>
<p>Salut à tous.</p> 
```
**Code CSS**
```css
p, h1 {
  color: blue;
  }
```
#### Appliquer un style : class et id
```
class: Utiliser un . devant le nom. Utilisable une seule Fois.
id:  : Utiliser un # devant le nom. Objet Unique.
```
**HTML**
```html
<div clss="TEST1"></div>
<div id="TEST2"></div>
```
**CSS**
```css
.TEST1 {
  }
#TEST1 {
  }
```
------------------------------------------------------------------------------------------------------------------------------------------
### [Formatez du texte](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605329-formatez-du-texte)
#### La taille
**La taille absolue**
```css
font-size: 16px;
```
**Une valeur relative**
```css
font-size: xx-small; /* minuscule   */
font-size: x-small;  /* très petit  */
font-size: small;    /* petit       */
font-size: medium;   /* moyen       */
font-size: large;    /* grand       */
font-size: x-large;  /* très grand  */
font-size: xx-large; /* Gigantesque */
```
#### La police
**Général**
```css
font-family: Verdana,arial;
```
**Police Personnalisée**
```css
@font-face {
  font-family: 'MaSuperPolice';
  src: url('MaSuperPolice.eot') format('eot'),
    url('MaSuperPolice.woff') format('woff'),
    url('MaSuperPolice.ttf') format('truetype'),
    url('MaSuperPolice.svg') format('svg');
}
```
#### Italique
```css
font-style: normal;
font-style: oblique;
font-style: italic;
```
**Gas**
```css
font-weight: bold;
```
**souligné**
```css
text-decoration: underline;    /* Souligné        */
text-decoration: line-through; /* barré           */
text-decoration: overline;     /* Ligne au-dessus */ 
text-decoration: none;         /* Normal (Défaut) */
```
#### L'alignement
```css
text-align: left;     /* Aligner le texte à Gauche    */
text-align: right;    /* Aligner le texte à Droite    */
text-align: center;   /* Aligner le texte à Centre    */
text-align: justify;  /* Aligner le texte à Justifier */
```

------------------------------------------------------------------------------------------------------------------------------------------
### [Ajoutez de la couleur et un fond](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605551-ajoutez-de-la-couleur-et-un-fond)
#### Couleur du texte ([ColorPicker](http://www.colorpicker.com/))
```css
color: maroon;
color: #FFFFFF;
color: rgb(240,96,204);
```
#### Couleur de fond
```css
background-color: black;
```
#### Images de fond
**XXX**
```css
background-image: url("neige.png");
```
#### La transparence
**XXX**
```css
```
**XXX**
```html
```
------------------------------------------------------------------------------------------------------------------------------------------
### []()
#### 
**XXX**
```html
```
**XXX**
```css
```




