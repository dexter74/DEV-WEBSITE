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
type='text'
type='email'
type='password'
type='url'
type='tel'
type='color'
type='number'
type='range'
type='search'

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
		<!-- ################################################################################################# -->
		<form method='post' action='connect.php'>
			<!-- ###########################################################################################  --->
			------------------------------------------------------------------------------------------------------
			<br />
			<label>Identifiant:</label>
				<input type='text' name='pseudo' maxlength='12' size='8' placeholder='Drthrax74240'/>
			<br />
			------------------------------------------------------------------------------------------------------
			<br />		
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Mot de passe:</label>
				<input type='password' name='password' maxlength='16' size='17' placeholder='Azerty74@1234567'/>
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Adresse Email:</label>
				<input type='email' name='password' maxlength='18' size='13' placeholder='teste74@hotmail.fr'/>
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Numéro de Téléphone:</label>
				<input type='tel' name='password' maxlength='10' size='7' placeholder='0765834177'/>
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Nationalité</label>
				<select>
						<option value='' selected></option>
					<optgroup label='Europe'>
						<option value='France' >France</option>
						<option value='Anglais'>Anglais</option>
						<option value='Espagne'>Espagne</option>
					</optgroup>
					
					<optgroup label='Amérique'>
						<option value='USA'>Etats-unis</option>
						<option value='Canada'>Canada</option>
						<option value='Texas'>Texas</option>
					</optgroup>
					
				</select>
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Date de Naissance:</label>
				<input type='date' name='naissance' />
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Votre page personnelle:</label>
				<input type='url' name='url' placeholder='http://www.localhost' maxlength='20' size='14' />
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Type de Jeux-Video:</label>
				<br />
				<input id='type' type="checkbox" name='mmorpg'/><label> MMORPG </label> 
				<br />
				<input id='type' type="checkbox" name='moba'/><label> MOBA </label> 
				<br />
				<input id='type' type="checkbox" name='fps'/><label> FPS </label> 
				<br />
				<input id='type' type="checkbox" name='str'/><label> STR </label> 
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			<label>Accepter la charte:</label>
				<br />
				<input id='type' type='radio' name='commun' value='NON'><label>NON</label>
				<input id='type' type='radio' name='commun' value='OUI'><label>OUI</label>	
			<!-- -------------------------------------------------------------------------------------------- --->
			<br />
			------------------------------------------------------------------------------------------------------
			<br />
			<label>Signature:</label>
				<br />
				<textarea maxlength='35'></textarea>
			<br />
			<!-- -------------------------------------------------------------------------------------------- --->
			------------------------------------------------------------------------------------------------------
			<br />
				<label>Moteur de recherche:</label>
				<br />
				<input id='search' type='search' />
			<br />
			------------------------------------------------------------------------------------------------------
			<!-- ############################################################################################ --->
		</form>
		<!-- ################################################################################################# -->
	</body>
</html>
```

```css
*   {
	margin: 0
	}
label{
	font-weight: bold;
	}
#type{
	margin-top: 5px;
	margin-left: 10px;
	}
textarea{
	margin-left:10px; 
	height:20px;
	width:350px;
	}
#search {
	margin-left:10px;
	height:20px;
	width:350px;
	}
 ```


---------------------------------------------------------------------------------------------------------------------------------------------------------------
### C. Le bouton d'envoi
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


---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> []()</p>


