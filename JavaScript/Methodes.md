#Methodes:

*Methodes die je kunt gebruiken in een string*

*https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/*
```javascript
//verandert alles in hoofdletters.
toUpperCase();
const string = "Hallo";
const upper = string.toUpperCase();
console.log(upper);
//veranders alles in kleine letters.
toLowerCase();
//Geeft het opgegeven nummer in de string terug, character at.
charAt();
//Geeft het indexnummer van de plek waarop het opgevraagde karakter het laatst voorkomt terug.
const string = "Hallo";
lastIndexOf("o"); //geeft 4 terug. 
//Returned alle karakters tussen de meegegeven indexnummers.
substring();
//Hakt de string in stukjes op basis van een conditie en returned de stukjes in een array.
const string = "Hallo";
const word = string.split("l");
console.log(word); // geeft ["Ha", "o"]
//of
const string = "Hallo mijn naam is Rianne";
const seperate = string.split(" "); 
console.log(seperate);// geeft ["Hallo", "mijn", "naam", "is", "Rianne"]
//Verwijdert spaties aan het begin en einde van een string.
trim();
//Vervangt alle instanties van de gespecificeerde karakters met iets anders.
replace();
//Checkt of de string een specifiek karakter(s) bevat.
includes();
```

*Methodes die je kunt gebruiken om te rekenen*

*https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math*
```javascript
//Bevat het wiskundige getal pi.
Math.pi();
//Rondt een getal af naar het dichtstbijzijnde hele getal
Math.round();
//Geeft de wortel van een getal terug.
Math.sqrt();
//Rondt een getal naar boven af.
Math.ceil();
//Rondt een getal naar beneden af.
Math.floor();
//Genereert een random getal tussen 0 en 1 - en is dus bij iedere aanroep anders!
Math.random();
```

*Methodes die je kunt gebruiken in een array*

*https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array*
```javascript
//Voegt twee arrays samen.
concat();
const array1 = [2, 3];
const array2 = [4, 5, 6];
array1.concat(array2); // geeft [2, 3, 4, 5, 6];
//Checkt of één van de items in de array een bepaalde waarde bevat, zoals “Lasagne bladen” of het getal 45. 
includes();
const array = [4, 5, 6];
array.includes(6); // geeft true
//Checkt het indexnummer van het item in de array met een bepaalde waarde, zoals “Lasagne bladen”.
indexOf();
const ingredients = ["Lasagne bladen", "Kaas", "Spinazie"];
ingredients.indexOf("Lasagne bladen"); // geeft 0
//Maakt een string van alle items in de array door ze achter elkaar te plakken. Wanneer je een argument meegeeft, zoals bijvoorbeeld een spatie, wordt deze tussen de items geplaatst.
join();
const words = ["Hoe", "gaat", "het"];
words.join(); // geeft "Hoegaathet"
words.join(" "); // geeft "Hoe gaat het"
words.join("-"); // geeft "Hoe-gaat-het"
//“pusht” een nieuw item, ofwel: voegt een item toe aan het einde van de array.
push();
const words = ["Hoe", "gaat", "het"];
words.push("?");
console.log(words); // geeft ["Hoe", "gaat", "het", "?"]
//Draait de volgorde van de array om.
const words = ["Hoe", "gaat", "het"];
words.reverse(); //geeft ["het", "gaat", "Hoe"]
//Verwijdert het laatste item in de array en returned deze waarde.
pop();
const ingredients = ["Lasagne bladen", "Kaas", "Spinazie"];
ingredients.pop(); // geeft "Spinazie" en de array is nu ["Lasagne bladen", "Kaas"]
//Verwijdert het eerste item in de array en returned deze waarde.
shift();
const ingredients = ["Lasagne bladen", "Kaas", "Spinazie"];
ingredients.shift(); // geeft "Lasagne bladen" en de array is nu ["Kaas", "Spinazie"]
//Maakt een referentieloze kopie van een deel van de array. 
// Dit betekent dat de originele array niet wordt aangepast. Dit kan handig zijn omdat je soms niet de originele array wil aanpassen,
//wat alle bovenstaande methodes wel doen.
slice();
const ingredients = ["Lasagne bladen", "Kaas", "Spinazie", "Eieren"];
ingredients.slice(); // kopieert de volledige array ["Lasagne bladen", "Kaas", "Spinazie", "Eieren"]
ingredients.slice(1); // kopieert vanaf positie 1, dus ["Kaas", "Spinazie", "Eieren"];
ingredients.slice(0, 1); // kopieert tussen positie 0 en 1 ["Lasagne bladen", "Kaas"];
//Voegt een item toe, vervangt of verwijderd een item op basis van indexnummer in de array. 
// Het is dus een hele diverse methode die op verschillende manieren gebruikt kan worden! Deze methode verwacht drie parameters:
//1. Het indexnummer (dus de positie) waar de operatie moet plaatsvinden
//2. Hoeveel items er verwijderd moeten worden (wil je niets weghalen? Dan vul je 0 in)
//3. Wat er toegevoegd moet worden (wil je niets toevoegen? Dan vul je 0 in)
splice();
//invoegen
const ingredients = ["Lasagne bladen", "Kaas", "Spinazie"];
// positie: 1, verwijderen: 0, toevoegen: "Eieren"
array.splice(1, 0, "Eieren") // geeft ["Lasagne bladen", "Eieren", "Kaas", "Spinazi"]
//vervangen
const ingredients = ["Lasagne bladen", "Kaas", "Spinazie"];
//positie: 1, verwijderen: 1, toevoegen: "Eieren"
array.splice(1, 1, "Eieren") // geeft ["Lasagne bladen", "Eieren", "Spinazie"]
//verwijderen
const ingredients = ["Lasagne bladen", "Kaas", "Spinazie"];
//positie: 2, verwijderen: 1, toevoegen: 0
array.splice(2, 1, 0) // geeft ["Lasagne bladen", "Kaas"]
```

*Date object*
```javascript
getTime() //geeft het aantal milliseconden dat zijn verstreken sinds de epoch 
getDay() //geeft de dag van de week (0 - 6) 
getHours() //geeft het uur (0 - 23) 
getMinutes()//geeft de minuten (0 - 59) 
getMonth() //geeft de maand (0 - 11) 
getSeconds() //geeft het aantal seconden (0 - 59)

const dateOfBirth = new Date(1992, 11, 26);
// Hier hebben we niet zoveel aan:
const englishDate = dateOfBirth.toDateString(); // geeft Sat Dec 26 1992
// Nederlandse versie voluit
const longOptions = {
    weekday: 'long',
    year: 'numeric',
    month: 'long',
    day: 'numeric',
};
const dutchDate = dateOfBirth.toLocaleDateString('nl-NL', longOptions); // geeft zaterdag 26 december 1992
// Nederlandse versie kort
const shortOptions = {
    weekday: 'short',
    month: 'long',
    day: 'numeric',
};
const dutchShortDate = dateOfBirth.toLocaleDateString('nl-NL', shortOptions); // geeft za 26 december
```
