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
	<h2>Formulaire d'inscription</h2>
	<form method='post' action='connect.php'>
		<fieldset>
			<label>Identifiant</label> 
				<input id='identifiant' type='text' name='username' size='14' maxlength='12' value='Drthrax74240' /> <br />
			
			<label>Mot de passe</label>
				<input id='motdepasse' type='password' name='password' size='14' maxlength='16' value='1234567890123456' /> <br />
			
			<label>Email</label>
				<input id='email' type='' name='mail' size='14' maxlength='18' value='teste74@hotmail.fr' /> <br />
			
			<label>Téléphone</label>
				<input id='telephone' type='tel' name='phone' size='14' maxlength='10' value='1234567890' /> <br />
			
			<label>Nationalité</label>
					<select id='pays'>
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
					
			<label>Charte</label>
				<input id='charte' type='radio' name='charte' value='OUI' /> Accepter |
				<input type='radio' name='charte' value='NON'/> Refuser
			<br />
			
			<label>Newsletter</label>
				<input id='newsletter' type='radio' name='newsletter' value='OUI' /> Accepter |
				<input type='radio' name='newsletter' value='NON'/> Refuser
			<br />
			
		</fieldset>
		
		
		
		<fieldset>
			<label>Page Perso</label>			
				<input id='pageperso' type='url' name='homepage' size='14' maxlength='21' value='http://192.168.1.2' /> <br />
			<label>Signature</label>
			<textarea id='signature' size='32' maxlength='170' placeholder='Contenue de ma signature numérique'></textarea>
		</fieldset>

		<fieldset>
		<label>Rechercher</label>
			<input id='' type='' name='' placeholder='' size='' maxlength='' value='' /> <br />
		</fieldset>	

	</form>
	
	<!-- ################################################################################################# -->
	</body>
</html>
```


```css
*{margin: 0}

/* Mise en forme du formulaire en général */
body{border: 5px black solid;padding: 2px;}
h2{border: 3px blue solid; margin-bottom: 5px;text-align:center}
form{}
label{font-weight: bold}
fieldset{border: 3px green solid; margin-bottom: 5px;}


/* Marge entre Label*/
#identifiant, #motdepasse, #email, #telephone, #pageperso{margin-bottom: 7px;}
#pays{margin-bottom: 20px;}
#charte{margin-bottom: 15px;}

/* Décalage des formulaires par rapport au label */
#identifiant{margin-left: 19.9px}
#motdepasse{margin-left: 3.9px}
#email{margin-left: 51.9px}
#telephone{margin-left: 21.7px}
#pays{margin-left: 17.0px}
#pays{width: 135px}
#charte{margin-left: 44.9px}
#newsletter{margin-left: 20px}
#pageperso{margin-left: 17.7px}
#signature{margin-left: 26.4px}
```

