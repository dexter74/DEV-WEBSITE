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
```
<table> </table>
```


#### 2. La balise En-tête
```
<th> </th>
```

#### 3. La balise de Ligne
```
<tr> </tr>
```

#### 4.La balise de Cellule
```
<td> </td>
```



#### 5. Mise en forme du tableau
```css

/* Bordures */
th{border: 1px black solid}
td{border: 1px solid black}

/* Coller les Cellules entre-elles */
table{border-collapse: collapse}
```





#### Exemple:
```html
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
table{border-collapse: collapse}
td{border: 1px black solid}
th{border: 1px black solid}
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
