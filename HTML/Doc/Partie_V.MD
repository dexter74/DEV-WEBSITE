---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> [Créez des formulaires](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1607171-creez-des-formulaires)</p>

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### A. Création d'un formulaire
#### 1. La Balise formulaire (HTML)
```html
<form></form>
```

#### 2. Regrouper les champs
```html
<fieldset> </fieldset>
```

#### 3. Les attributs
```html
method='post'        # Type de requête: Envoie
method='get'         # Type de requête: Réception 
action='connect.php' # Envoie la requête vers la page suivante
```
##### Exemple
```html
<form method='post' action='connect.php'></form>
```

#### 4. Libellés du contenu du formulaire (HTML)
```html
<label>Description du formulaire</label>
```

##### Exemple:
```html
<form method='post' action='connect.php'>
   <label>Description du formulaire</label>
</form>
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### B. Le contenu du formulaire (HTML)

#### 1. La balise Mono-Ligne
```html
<input />
```

#### 2. La balise Multi-Ligne (HTML, CSS)
```html
<textarea> </textarea>
```
```css
textarea{margin-left:10px; height:100px; width:500px;}
```

#### 3. Les attributs (HTML)
```html
type=''		# Définir le type de formulaire
id=''          	# Sert à identifier l'élément dans le HTML pour permettre sa manipulation
name=''        	# Name sert à la variable du formulaire. (Unique)
placeholder='' 	# Indication dans le formulaire directement
size=''        	# Taille du formulaire
maxlength=''   	# Nombre de caractère
value=''       	# Prédéfinir une valeur
autofocus	# Définis le champs qui sera en édite par défaut
required	# Champs obligatoire

#Number:
min=''
max=''  
step='' 
```

```css
:required{}
:focus{}
:invalid{}
```

#### 4. Type de formulaire
```html
type='text'		# Texte
type='email'		# Email
type='password'		# Mot de passe
type='url'		# URL
type='tel'		# Téléphone
type='number'		# Nombre (min='1' max='10' step='5')
type='color'		# Choix de couleur
type='range'		# Curseur
type='search'		# Rechercher
type='date'		# JJ/MM/AAAA
type='time'		# HH:MM
type='week'		# Semaine
type='month'		# Mois
type='datetime'		# Gestion du décalage
type='datetime-local'	# Heure locale

```

##### 5. Case à cocher (Multi-choix)
```html
type="checkbox"
```

##### 6. Case à cocher (Mono-choix)
```html
type='radio' name='commun' value='unique'
```

##### 7. Les listes déroulantes
###### Balise de base
```html
<select> </select>
```
###### Balise de Groupe
```html
<optgroup label=''> </optgroup>
```

###### Balise de choix
```html
# selected défini le choix par défaut
<option value='France' selected>France</option>
<option value='Anglais'>Anglais</option>
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### C. Le bouton d'envoi
#### 1. La balise de base
```
<input />
```

#### 2. Les attributs
```
type='submit'		# Bouton pour soumettre
type='image' src=''	# Bouton avec une image à la place
type='reset'		# Remise à zéro du formulaire

type='button'		# Bouton sans effet (A approfondir)
action=''		# Du formulaire (registered.php)
value=''       		# Prédéfinir une valeur
```

#### 3.
```
```

#### 4.
```
```

#### 5.
```
```



##### Exemple
```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title>Titre</title>
		<link rel="stylesheet" href="style.css" />
	</head>
	<body>
	<!-- ################################################################################################################################ -->
		<form method='post' action='inscription.php' >
			<fieldset>
				<h2>Formulaire d'inscription</h2>
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<div id='requis'>
					Champs obligatoire: *
				</div>
				<!-- <br /> -->
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Identifiant *</label>
					<input id='identifiant' type='text' name='username' size='14' maxlength='12' value='Drthrax74240' required autofocus />
					
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Mot de passe *</label>
					<input id='motdepasse' type='password' name='password' size='14' maxlength='16' value='1234567890123456' required />
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Email *</label>
					<input id='email' type='' name='mail' size='14' maxlength='18' value='teste74@hotmail.fr' required />
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Nationalité *</label>
						<select id='pays' required>
								<option value='country' ></option>
							<optgroup label='Europe'>
								<option value='France' selected>France</option>
								<option value='Anglais'>Anglais</option>
							</optgroup>
							<optgroup label='Amérique'>
								<option value='USA'>États-Unis</option>
								<option value='Canada'>Canada</option>
								<option value='Mexique'>Mexique</option>
							</optgroup>
						</select>
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Charte *</label>
					<input id='charte' type='radio' name='charte' value='OUI' required /> OUI |
					<input type='radio' name='charte' value='NON'/> NON
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Newsletter *</label>
					<input id='newsletter' type='radio' name='newsletter' value='OUI' required /> OUI |
					<input type='radio' name='newsletter' value='NON'/> NON
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Téléphone</label>
					<input id='telephone' type='tel' name='phone' size='14' maxlength='10' value='1234567890' />
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Page Perso</label>			
					<input id='pageperso' type='url' name='homepage' size='14' maxlength='21' value='http://192.168.1.2' />
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<label>Profile Steam</label>			
					<input id='steam' type='text' name='homepage' size='14' maxlength='21' value='http://192.168.1.2' />
				<br />
				<!-- -------------------------------------------------------------------------------------------------------------------- -->
				<input type='submit' value='Valider' />
				<input type='reset' value='Reset' />
			</fieldset>
			
		</form>

	<!-- ################################################################################################################################ -->
	</body>
</html>
```

```css
*{margin: 0}

/* Mise en forme du formulaire en général */
/* body{border: 5px black solid} */
h2, form, #requis{border: 2px green solid}
/* label{} */

/* Positionnement Texte */
h2{text-align:center}

/* Marge du titre du formulaire */
h2{
	margin-left: 50px;
	margin-right: 50px;
	margin-top: 2px;
	margin-bottom: 10px;
	}

/* Couleur de texte */
#requis{
	color: red;
	margin-bottom: 10px
	}

/* Marge entre élements */
#identifiant ,#motdepasse ,#email ,#pays ,#charte ,#newsletter ,#telephone ,#pageperso, #steam{margin-bottom: 10px}


/* Décalage des formulaires par rapport au label */
#identifiant{margin-left: 19.9px}
#motdepasse{margin-left: 2.2px}
#email{margin-left: 48.6px}
#pays{margin-left: 15.6px}
#charte{margin-left: 43.6px}
#newsletter{margin-left: 17px}
#telephone{margin-left: 31px}
#pageperso{margin-left: 28px}
#steam{margin-left: 11px}


/* Hauteur et Largeur*/
#pays{width: 135px}


:required
{
    background-color: #34495E;
}

/* :invalid */
/* { */
    /* background-color: #34495E; */
/* } */
```

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> [Enrichissez votre site avec de la vidéo et de l'audio](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1607438-enrichissez-votre-site-avec-de-la-video-et-de-laudio)</p>


#### 1.
```
```

#### 2.
```
```

#### 3.
```
```

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> [Utilisez le responsive design avec les Media Queries](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1607616-utilisez-le-responsive-design-avec-les-media-queries)</p>

#### 1. Méthode via le HTML
```css
<link rel="stylesheet" media="screen and (max-width: 1280px)" href="responsive.css" />
```

#### 2. Méthode via le CSS
```css
@media screen <règle> (max-width: 1280px){}
```

##### Combinaison de Règle
```css
only	: Uniquement
and	: Et
not	: N'est pas
```
###### Exemple
```css
/* Sur les écrans, quand la largeur de la fenêtre fait au maximum 1280px */
@media screen and (max-width: 1280px)

/* Sur tous types d'écran, quand la largeur de la fenêtre est comprise entre 1024px et 1280px */
@media all and (min-width: 1024px) and (max-width: 1280px)

/* Sur les téléviseurs */
@media tv

/* Sur tous types d'écrans orientés verticalement */
@media all and (orientation: portrait)
```


#### 3. Règle disponible CSS
```
color: 			# Couleur
height:			# Hauteur
width:			# Largeur
device-height:		# Hauteur du périphérique
device-width:		# Largeur du périphérique
orientation:		# portrait ou paysage

media: screen;		# Ecran Classique (PC)
media: handheld;	# Périphértique Mobile
media: print;		# Impression
media: tv;		# Télévision
media: projection;	# Projecteur
media: all;		# Tous les types d'écrans

Préfix possible: 
 min-XXXX		# Exemple: min-width
 max-XXXX		# Exemple: max-width
```

#### 4.
```
```

#### 5.
```
```

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> []()</p>

#### 1.
```
```

#### 2.
```
```
#### 3.
```
```

#### 4.
```
```

#### 5.
```
```

