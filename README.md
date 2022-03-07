# TP Cinema
but : Créer une maquette de site web sur le thème des sites de streaming  
Rendez-vous sur [TP-cinema](https://lahuts.github.io/tpcinema/index.html) pour voir l'aperçu!
## Index
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./css/reset.css">
    <link rel="stylesheet" href="./css/main.css">
    <link rel="icon" type="favicon"  href="favicon/favicon.ico">
    <title>TP Cinema</title>
    
</head>
<body>
    <header>
        <a href="index.html"><img src="asset/logo.svg" alt="logo du site"></a>
        <h1>Films , séries TV et bien plus en illimité !</h1>
    </header>
    <main>
        <section>
            <h2>Prêt à regarder ? Remplissez le formulaire proposé dans cette page </h2>
            <p>Tous les mois profitez de toutes les nouveautés série et cinéma. A partir du mois
                prochain on vous propose tous les classiques du cinéma. Où que vous soyez. Tous
                les films en VO, VOST, VF et plus d'options</p>
        </section>
        <section>
            <ol>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
            </ol>
        </section>
        <a href="formulaire.html"><p>Cliquez ici pour commencer</p></a>
    </main>
    <footer><p>@ - Streaming - 2022</p></footer>
</body>
</html>

```
## Css Main
```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500;700&display=swap');
body{
    font: 1.6rem;
    font-family: 'Roboto', sans-serif;
    background-color: rgb(54, 53, 53);
    color: #fff;
    background-image: url(https://images.unsplash.com/photo-1578662996442-48f60103fc96?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80);
}

header{
    text-align: center;
    overflow: hidden;
}
header>a>img{
    width: 10rem;
    height: 10rem;
}
header>h1{
    margin-bottom: 2rem;
    font-size: xx-large;
    font-weight: 700;
    color: #fff;
}


main{
    margin-left: 16rem;
    margin-right: 16rem;
}
section>h2{
    font-weight: 500 ;
    text-align: center;
    font-size: 2rem;
}
section>p{
    font-size: medium;
    margin-top: 1rem;
    text-align: center;
    font-size: 1.6rem;
}
ol{
    display: grid;
    grid-template-columns: repeat(5,1fr);
    margin-top: 2em;
    float: left;
    


}
li{
    width: 10rem;
    height: 14.5rem;
}
a{
    margin-top: 2em;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1rem;
    
    
}
a>p{
    text-align: center;
    color: #fff;
    font-size:large;
    font-weight: 500;
    background-color: rgba(255, 26, 18,1);
    padding: 0.5em;
    padding-left: 5em;
    padding-right: 5em;
    transition: background-color 0.5s;
}
a>p:hover{
     background-color: rgba(255, 26, 18, 0.5); ;
}
section:nth-child(2){
    overflow: hidden;
    display: flex;
    justify-content: center;
}
li{
    margin: 1em;
}
li>img{
    width: 100%;
}
footer{
    margin-top: 2rem;
}
footer>p{
    text-align: center;
}
```

## html page formulaire
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./css/reset.css">
    <link rel="stylesheet" href="./css/form.css">
    <link rel="icon" type="favicon"  href="favicon/favicon.ico">
    <title>TP Cinema</title>
    
</head>
<body>
    <header>
        <img src="asset/logo.svg" alt="logo du site">
        <h1>Films , séries TV et bien plus en illimité !</h1>
    </header>
    <main>
        <section>
            <ol>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
                <li><img src="asset/django.jpg" alt="affiche django"></li>
            </ol>
        </section>

        <form action="">
            <h2>Remplissez le formulaire :</h2>
            <label for="nom">Nom :</label>
            <input type="text" name="nom">
            <label for="prenom">Prénom :</label>
            <input type="text"name=prenom>
            <label for="email">Email :</label>
            <input type="email" name="" id="">
            <label for="pays">Pays :</label>
            <select name="pays" id=""></select>
            <label for="ville">Ville :</label>
            <select name="ville" id=""></select>
            <input type="button" value="Valider">
        </form>
    </main>
    <footer><p>@ - Streaming - 2022</p></footer>
</body>
</html>
```
## Css form 
```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500;700&display=swap');
body{
    font: 1.6rem;
    font-family: 'Roboto', sans-serif;
    background-color: rgb(54, 53, 53);
    color: #fff;
    background-image: url(https://images.unsplash.com/photo-1578662996442-48f60103fc96?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80);
}
header{
    overflow: hidden;
    text-align: center;
}
header>h1{
    font-size: xx-large;
    font-weight: 700;
    color: #fff;
}

header>a>img{

    width: 10rem;
    height: 10rem;
}
section:nth-child(1){
    overflow: hidden;
    display: flex;
    justify-content: center;
}
ol{
    display: grid;
    grid-template-columns: repeat(5,1fr);
    margin-top: 2em;
    float: left;
    


}
li{
    width: 10rem;
    height: 14.5rem;
    margin: 1em;
}
li>img{
    width: 100%;
}
section{
    overflow: hidden;
}
main{
    margin-left: 16rem;
    margin-right: 16rem;
}
form{
    display: flex;
    width: 100%;
    line-height: 4em;
    flex-direction: column;
    align-items: center;

}
form>h2{text-align: center;}
label,select,input{
    margin-left: 1rem;
}
label{
    display: block;
    font-size:medium;
}
h2{
    font-size: x-large;
    font-weight: 500;
}
input,select{
    background-color: rgba(77, 75, 75, 0.748);
    width: 35rem;
    height: 4rem;
    border-radius: 0.7rem 0.7rem 0.7rem 0.7rem;
    color:#fff;
    padding: 1em;
}
input:last-child{
    margin-top: 3rem;
    background-color: rgba(255, 26, 18,1);
    transition: background-color 0.5s;
}
input:last-child:hover{
    background-color: rgba(255, 26, 18, 0.5); ;
}

footer{
    margin-top: 2rem;
    margin-bottom: 2rem;
}
footer>p{
    text-align: center;
}
```