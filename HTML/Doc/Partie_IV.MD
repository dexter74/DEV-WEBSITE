---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> [Ajoutez des tableaux](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1606851-ajoutez-des-tableaux)</p>


### Structure de base d'une page HTML
```
<!DOCTYPE html>
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
```

### A. Un tableau simple
#### 1. Les balises de base
```php
<table> </table>
```
```css
table{border-collapse: collapse}
```

#### 2. Titre du tableau
```php
<caption></caption>
```
```css
caption{
	caption-side: top;		/* Titre au-dessus  du Tableau */
	caption-side: bottom;		/* Titre en-dessous du Tableau */
	border: 1px black solid;	/* Bordure */
	}
```
#### 3. La balise de Ligne
```php
<tr> </tr>
```
#### 4. La balise En-tête
```php
<th> </th>
```
```css
th{border: 1px black solid}
```
#### 5.La balise de Cellule
```php
<td> </td>
```
```css
td{border: 1px black solid}
```
#### Exemple:
```php
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title>Titre</title>
		<link rel="stylesheet" href="style.css" />
	</head>
	<body>
		<table>
			<!-- ############################################ -->
			<caption>Base de donnée des utilisateurs</caption>
			<!-- ############################################ -->
			<tr>
				<th>ID</th>
				<th>User</th>
				<th>Password</th>
				<th>Prénom</th>
				<th>Nom</th>
				<th>Age</th>
				<th>Email</th>
				<th>Activation</th>
				<th>Permission</th>
			</tr>
			<!-- ############################################ -->
			<tr>
				<td>0</td>
				<td>Drthrax74</td>
				<td>Passw0rd2022</td>
				<td>Marc</td>
				<td>Jaffré</td>
				<td>31</td>
				<td>teste74@hotmail.fr</td>
				<td>enabled</td>
				<td>Administrateur</td>
			</tr>
			<!-- -------------------------------------------- -->
			<tr>
				<td>1</td>
				<td>Stitch74</td>
				<td>Passw0rd2022</td>
				<td>Fabrice</td>
				<td>Jaffré</td>
				<td>31</td>
				<td>Drthrax74@hotmail.fr</td>
				<td>enabled</td>
				<td>Administrateur</td>
			</tr>
			<!-- ############################################ -->
		<table>
	</body>
</html>
```
```css
/* Cellule collé entre-elles */
table{border-collapse: collapse}

/* Titre du tableau au dessus */
caption{caption-side: top;border: 1px black solid;font-weight: bold;}

/* Bordure sur la balise En-tête */
th{border: 1px black solid}

/* Bordure sur la balise de Cellule */
td{border: 1px black solid}
```




---------------------------------------------------------------------------------------------------------------------------------------------------------------

### B. Un tableau structuré (Gros Tableau)

#### 1. En-tête
```php
<thead></thead>
```
#### 2. Corps
```php
<tfoot> </tfoot>
```
#### 3. Pied de tableau
```php
<tbody> </tbody>
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
		<table>
			<!-- ############################################ -->
			<caption>Base de donnée des utilisateurs</caption>
			<!-- ############################################ -->
			<thead>
				<tr>
					<th>ID</th>
					<th>User</th>
					<th>Password</th>
					<th>Prénom</th>
					<th>Nom</th>
					<th>Age</th>
					<th>Email</th>
					<th>Activation</th>
					<th>Permission</th>
				</tr>
			</thead>
			<!-- ############################################ -->
			<tbody>
			<tr>
				<td>0</td>
				<td>Drthrax74</td>
				<td>Passw0rd2022</td>
				<td>Marc</td>
				<td>Jaffré</td>
				<td>31</td>
				<td>teste74@hotmail.fr</td>
				<td>enabled</td>
				<td>Administrateur</td>
			</tr>
			<!-- -------------------------------------------- -->
			<tr>
				<td>1</td>
				<td>Stitch74</td>
				<td>Passw0rd2022</td>
				<td>Fabrice</td>
				<td>Jaffré</td>
				<td>31</td>
				<td>Drthrax74@hotmail.fr</td>
				<td>enabled</td>
				<td>Administrateur</td>
			</tr>
			<!-- ############################################ -->
			<tfoot>
				<tr>
					<th>ID</th>
					<th>User</th>
					<th>Password</th>
					<th>Prénom</th>
					<th>Nom</th>
					<th>Age</th>
					<th>Email</th>
					<th>Activation</th>
					<th>Permission</th>
				</tr>
			</tfoot>
			
			
			</tbody>
			
		<table>
	</body>
</html>
```
#### 4. Fusion
```
Pour effectuer une fusion, on rajoute un attribut à la balise <td>
```

##### Fusion de colonnes
```
Il faut utiliser colspan puis définir le nombre de colonne à fusionnées.

<td colspan="X">
```

##### Fusion de lignes
```
Il faut utiliser rowspan puis définir le nombre de colonne à fusionnées.
<td rowspan="X">
```

###### Exmple
```
```










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
