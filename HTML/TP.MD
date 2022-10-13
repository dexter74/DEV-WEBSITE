## Tableau 
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

```
*{margin: 0}
body{
	background-color: #131313;}
/* Cellule collé entre-elles */
table{border-collapse: collapse}
table{margin: auto}

/* Titre du tableau au dessus */
caption{
	caption-side: top;
	/* border: 1px white solid; */
	font-weight: bold;
	color: red;
	margin-bottom: 10px;
	line-height: 70px;	
	}

/* Bordure sur la balise En-tête */
th{
	border: 1px white solid;
	font-weight: bold;
	color: green;
	width: 200px;
	line-height: 30px;
}

/* Bordure sur la balise de Cellule */
td{border: 1px white solid;
	font-weight: bold;
	color: white;
	text-align: center;

	line-height: 25px;	
	}
