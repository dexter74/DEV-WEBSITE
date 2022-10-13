---------------------------------------------------------------------------------------------------------------------------------------------------------------
## <p align='center'> [Ajoutez des tableaux](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1606851-ajoutez-des-tableaux)</p>


### Structure de base d'une page HTML
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Titre</title>
        <link rel="stylesheet" href="style.css" />
    </head>
    <header></header>
    <body></body>
    <footer></footer>
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

<br />

#### 2. Titre du tableau
```php
<caption></caption>
```
```css
caption{
	caption-side: top;	/* Titre au-dessus  du Tableau */
	caption-side: bottom;	/* Titre en-dessous du Tableau */
	}
```

<br />

#### 3. La balise En-tête
```php
<th> </th>
```
```css
th{border: 1px black solid}
```

<br />

#### 4. La balise de Ligne
```php
<tr> </tr>
```

#### 5.La balise de Cellule
```php
<td> </td>
```
```css
td{border: 1px black solid}
```

<br />


#### Exemple:
```php
		<table>
			<!-- ########################### -->
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
			<!-- ########################### -->
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
			<!-- --------------------------- -->
			<!-- ########################### -->

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
			<!-- ########################### -->
		<table>
```

```css

td{border: 1px black solid}

```





### B. Un tableau structuré
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
