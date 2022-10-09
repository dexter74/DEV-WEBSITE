---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'> [Structurez votre page](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605881-structurez-votre-page)</p>

#### A. Les balises structurantes de HTML5
###### 1. En-tête
```html
<header></header>
```

###### 2. Le pied de page
```html
<footer></footer>
```

###### 3. Les principaux liens de navigation 
```html
<nav>
    <ul>
        <li><a href="index.html">Accueil</a></li>
        <li><a href="forum.html">Forum</a></li>
        <li><a href="contact.html">Contact</a></li>
    </ul>
</nav>
```

###### 4. Une section de page
```html
<section>
    <h1>Ma section de page</h1>
    <p>Bla bla bla bla</p>
</section>
```

###### 5. Informations complémentaires
```html
<aside></aside>
```

###### 6. Un article indépendant
```html
<article>
    <h1>Mon article</h1>
    <p>Bla bla bla bla</p>
</article>
```

<p align="center"><img src="https://user-images.githubusercontent.com/35907/194761512-8fe17e2f-450f-440d-9ff0-e3aa81f8f360.png" alt="Sublime's custom image"/></p>

---------------------------------------------------------------------------------------------------------------------------------------------------------------
###### Exemple 
L'image au dessus n'est pas représentative du code suivant.
```html
<!DOCTYPE html>
<html>
	<!-- ################################################################### -->
    <head>
        <meta charset="utf-8" />
        <title>Titre</title>
        <link rel="stylesheet" href="style.css" />
    </head>
	<!-- ################################################################### -->
    <header>
		<h1>Titre de mon site</h1>
	</header>
	<!-- ################################################################### -->
    <body>
		<div id="Menu">
			<nav>
				<ul>
					<li><a href="index.html">Accueil</a></li>
					<li><a href="forum.html">Forum</a></li>
					<li><a href="contact.html">Contact</a></li>
				</ul>
			</nav>
		</div>
	</body>
	<!-- ################################################################### -->
   	<footer>
		<p>Copyright, Tous droits réservés .</p>
	</footer>
	<!-- ################################################################### -->

</html>
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'>[Découvrez le modèle des boîtes](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1606168-decouvrez-le-modele-des-boites)</p>

#### A. Les balises de type block et inline
###### 1. Les Balises Block
`Une balise Block fait un Retour à la ligne avant et après.`
```html
<p></p>
<div></div>
```
###### 2. Les Balises Inline
`Une balise Inline est dans une balise Block. Elle ne fait pas de retour à la ligne.`
```html
<a></a>
<span></span>
```
**Exemple**
```html
<p> Mon block contient  le bloc "<a/>INLINE</a>" dans son contenu. </p>
```
###### 3. Les balises universelles
```
Class et ID
```
#### B. Les dimensions (Balise Block)
###### 1. Hauteur
```css
height: 0px ou X%;  /* Hauteur du Bloc  */
min-height: 0px;    /* Hauteur Minimale */ 
max-height: 0px;    /* Hauteur maximale */
```
###### 2. Largeur
```css
width: 0px ou 0%;  /* Largeur du Bloc  */
min-width: 0px;    /* Largeur Minimale */ 
max-width: 0px;    /* Largeur maximale */
```

#### C. Les marges
<p align="center"> <img src="https://user-images.githubusercontent.com/35907/194766690-b5c487d0-912d-43ab-914c-4531a8051baa.png" alt="Sublime's custom image"/></p>

###### 1. Intérieur
```css
padding: 0px;		/* Indique la taille de la marge intérieure. À exprimer en général en pixels (px) */
padding-top: 0px;	/* Marge intérieure en haut 	*/
padding-bottom:	0px;	/* Marge intérieure en bas 	*/
padding-left: 0px;	/* Marge intérieure à gauche 	*/
padding-right: 0px;	/* Marge intérieure à droite 	*/
```
###### 2. Extérieur
```css
margin: 2px 0 3px 1px;	/* Marge Extérieur des 4 côtés	*/
margin-top: 0px; 	/* Marge extérieure en haut 	*/
margin-bottom: 0px; 	/* Marge extérieure en bas 	*/
margin-left: 0px; 	/* Marge extérieure à gauche 	*/
margin-right: 0px; 	/* Marge extérieure à droite	*/
```

###### 3. Centrer Bloc
```css
margin: auto;	/* Requiert: width */
width: 0px;
```
#### E. Quand ça dépasse…
###### 1. Couper un bloc
```css
overflow: visible;	/* Le texte sera visible et celui-ci sort volontairement du bloc */
overflow: hidden;	/* Le texte sera tout simplement coupé Net. */
overflow: scroll;	/* Le texte sera tout simplement coupé avec barre de navigation */
overflow: auto;		/* Mode Automatique gérer par le navigateur */
```
###### 2. Couper les textes trop larges
```css
word-wrap: break-word; /*  Cette propriété permet de forcer la césure des très longs mots */
```









---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'>[Faites votre mise en page avec Flexbox](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/3298561-faites-votre-mise-en-page-avec-flexbox)</p>

#### A. Un conteneur, des éléments
<p align="center"> <img src="https://user-images.githubusercontent.com/35907/194774895-ccafba54-7a31-4aec-a01c-1196fea91b76.png" alt="Sublime's custom image"/></p>

<p align="center"> <img src="https://user-images.githubusercontent.com/35907/194774944-403707f8-503c-487d-8148-54f830a69827.png" alt="Sublime's custom image"/></p>

#### B. Soyez flex !
###### 1. Activer le mode Flex
Sans autre propritété l'orientation est vers la droite.
```css
display: flex;	/* Permet d'activer le mode FlexBox */
```

###### 2. La direction (Conteneur)
On peut les positionner verticalement ou encore les inverser
```css
flex-direction: row;		/* Organisés sur une ligne				*/
flex-direction: column;		/* Organisés sur une colonne			 	*/
flex-direction: row-reverse;	/* Organisés sur une ligne, mais en ordre inversé	*/
flex-direction: column-reverse;	/* Organisés sur une colonne, mais en ordre inversé	*/
```
###### 3. Le retour à la ligne
```css
flex-wrap: nowrap;		/* Pas de retour à la ligne 				*/
flex-wrap: wrap;		/* Retour à la ligne si plus de place 			*/
flex-wrap: wrap-reverse;	/* Retour à la ligne si plus de place (Sens Inverse)	*/
```


#### C. Alignez-les !
###### 1. Aligner sur l'axe principal (Horizontal)
```css
justify-content: flex-start;	/* Alignés au début						*/
justify-content: flex-end;	/* Alignés à la fin						*/
justify-content: center;	/* Alignés au centre						*/
justify-content: space-between;	/* Les éléments sont étirés sur tout l'axe (Espace entre eux)	*/
justify-content: space-around;	/* Idem, laisse de l'espace sur les extrémités			*/
```

###### 2. Aligner sur l'axe secondaire (Vertical)
```css
align-items:stretch;		/* Les éléments sont étirés sur tout l'axe (valeur par défaut)	*/
align-items:flex-start; 	/* Alignés au début						*/
align-items:flex-end; 		/* Alignés à la fin 						*/
align-items:center;		/* Alignés au centre						*/
align-items:baseline;		/* Alignés sur la ligne de base (semblable à flex-start)	*/ 
```

###### 3. Aligner un seul élément
```html
<div id="conteneur">
    <div class="element 1">Accueil</div>
    <div class="element 2">Forum</div>
</div>
```
```css

/* Conteneur */
#conteneur{}

/* Élément 1: XXXX */
.element:nth-child(1){}

/* Élément 2: XXXX */
.element:nth-child(2){}
```

#### D. Répartir plusieurs lignes
```
Tutorial Incomplet ou pas pertinent
```


#### E. Rappel à l'ordre
###### 1. Définir un Ordre dans les éléments
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Titre</title>
        <link rel="stylesheet" href="style.css" />
    </head>
    <body>
		<div id="conteneur">
			<div class="element 1">Foot</div>
			<div class="element 2">Bandeau</div>
			<div class="element 3">Header</div>
		</div>
    </body>
</html>
```

```css
/* Configuration de la page par défaut */
*{margin: 0;}

/* Conteneur */
#conteneur{display: flex;}

/* Éléments: Pied de Page */
.element:nth-child(1){border: 1px blue solid}
.element:nth-child(1){margin: 1px;}
.element:nth-child(1){order: 3;}

/* Éléments: Bandeau*/
.element:nth-child(2){border: 1px red solid}
.element:nth-child(2){margin: 1px;}
.element:nth-child(2){order: 1;}

/* Éléments: Header */
.element:nth-child(3){border: 1px green solid}
.element:nth-child(3){margin: 1px;}
.element:nth-child(3){order: 2;}
```

#### F. Encore plus flex : faire grossir ou maigrir les éléments
###### 1. Un élément
```css
flex: 1;
```

###### 2. Plusieurs éléments avec proportion
```css
.element:nth-child(1){flex: 2;}
.element:nth-child(2){flex: 1;}
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align='center'>[]()</p>

#### A. 
###### 1. 
```html
```
