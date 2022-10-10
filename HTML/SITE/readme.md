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
		<div id='SITE'>
			<div id='TOP'></div>
			<!-- ############################# -->
			<div id='CORPS'></div>
			<!-- ############################# -->
			<div id='GAUCHE'>
				<div class='Module_1'></div>
				<div class='Module_2'></div>
				<div class='Module_3'></div>
			</div>
			<!-- ############################# -->
			<div id='MILIEU'>
				<div class='HAUT'></div>
				<div class='BAS'></div>
			</div>
			<!-- ############################# -->
			<div id='DROITE'></div>
			<!-- ############################# -->
		</div>
	<body>
</html>
```

