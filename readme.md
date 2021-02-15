# Introduction

L'objectif du document est la création d'une *cheat sheet* ou "feuille de triche". 

L'ensemble des fonctions que vous devez documenter se trouvent dans ce document, à vous de  remplir les espaces vides 😉

Ce document pourra vous suivre tout au long de vos études, n'hésitez à le compléter au fur et à mesure.

---

Pour compléter le document, vous utiliserez la fonction **fork** de GitHub pour copier ce projet dans votre espace personnel.

[Si besoin, rendez-vous dans ce dépôt pour revoir les bases de Javascript](https://github.com/Maxence-Machu/javascript-basic-memo)

---

## La fonction GetElementByID()

### Que fait la fonction ?
La méthode getElementById() renvoie un objet qui représente l'élément dont la propriété  id correspond à la chaîne de caractères spécifiée.
Étant donné que les ID d'élément doivent être uniques, s'ils sont spécifiés, ils constituent un moyen utile d'accéder rapidement à un élément spécifique.

### Pourquoi l'utiliser ?
La fonction getElementById doit être utilisée si l'on veut utiliser un élément du DOM en HTML grâce à Javascript 

#### Note supplémentaire
La fonction getElementByID est à ne pas confondre avec la fonction *getElementsByClassName*. 
Les ID dans une page web sont uniques, on ne peut donc pas récupérer plusieurs éléments avec cette fonction. 

### Exemple de code:
```javascript
let element = document.getElementByID('mon-element');
console.log(element);
```

## La fonction GetElementsByClassName()

### Que fait la fonction ?
La méthode getElementById() renvoie un objet de type tableau qui représente l'élément dont la propriété  de tous les éléments enfants qui ont tous les noms de classe donnés.
Lorsqu'il est appelé sur l'objet document, le document complet est recherché, y compris le nœud racine.

### Pourquoi l'utiliser ?
La fonction getElementClassName() doit être utilisée si l'on veut utiliser un ou plusieurs éléments du DOM en HTML grâce à Javascript

### Exemple de code:
```javascript
var element = document.getElementsByClassName('test');
console.log(element);
```

## La fonction querySelector() et querySelectorAll()

### Que fait la fonction ?
La méthode querySelector() de l'interface Document retourne le premier Element dans le document correspondant au sélecteur - ou groupe de sélecteurs - spécifié(s), ou null si aucune correspondance n'est trouvée. En revanche, querySelectorAll() de Element renvoie une NodeList statique représentant une liste des éléments du document qui correspondent au groupe de sélecteurs spécifiés.

### Pourquoi l'utiliser ?
Si le sélecteur correspond à un ID et que cet ID est utilisé de façon erronée plusieurs fois dans le document, le premier élément en correspondance est retourné.
Si vous avez besoin d'une liste de tous les éléments correspondant aux sélecteurs spécifiés, vous devez utiliser querySelectorAll() à la place.
### Exemple de code:
```javascript
var el = document.querySelector(".maclasse");
console.log(el);
var matches = document.querySelectorAll("p");
console.log(matches);
```

## La fonction addEventListener()

### Que fait la fonction ?
La méthode addEventListener() installe une fonction à appeler chaque fois que l'événement spécifié est envoyé à la cible. Les cibles courantes sont un Element, le Document lui-même et une Window.

### Pourquoi l'utiliser ?
Cette méthode s'utilise pour ajouter un événement sur un élément du DOM

### Exemple de code:
```javascript
document.getElementById("myBtn").addEventListener("click", function() {
  document.getElementById("demo").innerHTML = "Hello World";
});
```

## La fonction stopPropagation()

### Que fait la fonction ?
Cette méthode va stopper la propagation d’un évènement après qu’un gestionnaire d’évènement (gérant l’évènement en question) ait été atteint.

### Pourquoi l'utiliser ?
On l'utilise pour stopper un l'événement en cours en remontant à l'élément parent

### Exemple de code:
```javascript
function func1(event) {
  alert("DIV 1");
  event.stopPropagation();
}
```

## La fonction addEventListener('mousemove', maFonction)

### Que fait la fonction ?
La fonction s'effectue lorsque la souris passe sur l'endroit ou est établie maFonction

### Pourquoi l'utiliser ?
On l'utilise pour crée une animation 

### Exemple de code:
```javascript
document.getElementById("element").addEventListener("mousemove", MaFonction() {
  document.getElementById("demo").innerHTML = "Hello World";
```

## La fonction parseInt()

### Que fait la fonction ?
La fonction parseInt() analyse une chaîne de caractère fournie en argument et renvoie un entier exprimé dans une base donnée.

### Pourquoi l'utiliser ?
Cette méthode est utilisée pour retrouve des valeurs dans un chaine de caractères

### Exemple de code:
```javascript
var age = parseInt("40 years")
console.log(age);
```


## La variable "event" dans le code suivant:

### Code:
```javascript
element.addEventListener('event-name', function(event) {
  console.log(event);
});
```

### Qu'est-ce que cette variable ?
...

### Pourquoi l'utiliser ?
...


