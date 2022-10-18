---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> [Créez des formulaires](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1607171-creez-des-formulaires)</p>

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### A. Création d'un formulaire

#### 1. La Balise formulaire
```html
<form></form>
```
#### 2. Les attributs
```html
method='post'        # Type de requête: Envoie
method='get'         # Type de requête: Réception 
action='connect.php' # Envoie la requête vers la page suivante
```
##### Exemple
```html
<form method='post' action='connect.php'></form>
```

#### 3. Libellés du contenu du formulaire
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
### B. Le contenu du formulaire
#### 1. La balise Mono-Ligne
```html
<input />
```

#### 2. La balise Multi-Ligne
```html
<textarea> </textarea>
```
```css
textarea{margin-left:10px; height:100px; width:500px;}
```

#### 3. Les attributs
```html
type=''
id=''          # Sert à identifier l'élément dans le HTML pour permettre sa manipulation
name=''        # Name sert à la variable du formulaire. (Unique)
placeholder='' # Indication dans le formulaire directement
size=''        # Taille du formulaire
maxlength=''   # Nombre de caractère
value=''       # Prédéfinir une valeur


#Number:
min=''
max=''  
step='' 
```

#### 4. Type de formulaire
```html
type='color'
type='email'
type='number'
type='password'
type='range'
type='text'
type='search'
type='tel'
type='url'

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

##### 5. Case à cocher (Mono-choix)
```html
type='radio' name='commun' value='unique'
```












##### Exemple
```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title>Titre</title>
		<link rel="stylesheet" href="style.css" />
	</head>
	<body>
	<!-- --------------------------------------------------------------------------- -->
		<!-- ####################################################################### -->
		<form method='post' action='connect.php'>
			<h2>Inscription:</h2>
			<label>Identifiant: </label>
			<input type='text' id='pseudo' name='username' size='8' maxlength='12' />
			<br />
			<label>Mot de passe: </label>
			<input type='password' id='mdp' name='password' size='8' maxlength='12' />
			<br />
			<br />
			<label>Votre signature:</label>
			<br />
			<textarea type='text' height='100' ></textarea>
			<br />
			<label>Accepter le CLUF: </label>
			<br />
			<input id='CLUF' type="checkbox" name="choix" ><label> Test </label>
		</form>
		<!-- ####################################################################### -->
	<!-- --------------------------------------------------------------------------- -->
	</body>
</html>
 ```
 ```css
*{margin: 0}
label{font-weight: bold;}
textarea{margin-left: 10px;height: 100px;width: 500px;}	
#CLUF{margin-top: 5px;margin-left: 20px}
 ```


### B. 
```
```
### C. 
```
```
### D. 
```
```



---------------------------------------------------------------------------------------------------------------------------------------------------------------
### D. Les éléments d'options


<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
### E. Finaliser et envoyer le formulaire

<br />

---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> []()</p>

### A.
### B.
### C.
### D.
### E.


#### 1.
#### 2.
#### 3.
#### 4.
#### 5.

```
```
