------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## <p align='center'>Conception du site</a>

------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<p align='center'>
  <img src='https://user-images.githubusercontent.com/35907/194784647-e20235f5-4adb-4c31-964f-12c8c709e7ab.png'/>
</a>


#### Eléments:
```
ID: SITE
 > ID: TOP
 > ID: CORPS
  > ID: GAUCHE
   > CLASS: MODULE_1
   > CLASS: MODULE_2
   > CLASS: MODULE_3
  > ID: MILIEU
   > CLASS: HAUT
   > CLASS: BAS
  > ID: DROITE
```

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Website par Marc Jaffré</title>
        <link rel="stylesheet" href="style.css" />
    </head>
	<body>
		<div id='TOP'>
			<div class='MENU 1'>ACCUEIL</div>
			|
			<div class='MENU 2'>FORUM</div>
			|
			<div class='MENU 3'>SUPERVISION</div>
			|
			<div class='MENU 4'>SUPPORT</div>
		</div>
		<div id='MID'>
			<div class='MILIEU 1'>GAUCHE</div>
			<div class='MILIEU 2'>
				<div class='TITRE'>TITRE</div>
				<div class='CONTENU'>CONTENU</div>
			</div>
				<div class='MILIEU 3'>DROITE</div>
		</div>
				<div id='BAS'>Copyright</div>
	<body>
</html>
```

```css
/* https://www.w3schools.com/css/tryit.asp?filename=trycss3_flexbox_responsive2	 */
*{
	margin: 0;
	box-sizing: border-box;
	}
/* ----------------------------------------------------------------------------- */
body{
	background-color: #DAF7A6;
	}
/* ----------------------------------------------------------------------------- */
#TOP{
	display: flex;flex-wrap: wrap;
	line-height: 200%;
	font-size: 140%;
	margin-bottom: 20px;
	color: white;
	background-color: black;
}

.MENU:nth-child(1){margin: auto}
.MENU:nth-child(2){margin: auto}
.MENU:nth-child(3){margin: auto}
.MENU:nth-child(4){margin: auto}


/* ----------------------------------------------------------------------------- */
#MID{
	display: flex;
	flex-wrap: wrap;
	margin-bottom: 30px;
	min-height: 300px;

	margin: 5px;
}

#BAS{
	background-color: black;
	text-align: center;
	color: white;
}


/* Gauche */
.MILIEU:nth-child(1){width: 15%   ;margin-right: 0.3%; background-color: cyan;}

/* Milieu */
.MILIEU:nth-child(2){width: 69.4%;background-color: green;}
.TITRE{text-align: center;}
.CONTENU p{text-align: justify; font-size: 100%;}
/* Droite */
.MILIEU:nth-child(3){width: 15%;margin-left: 0.3%; background-color: red;}

```
