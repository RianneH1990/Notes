#Functies

###Functies declareren:
*Function is een stukje code dat je herhaaldelijk kunt gebruiken. Je schrijft het een keer en daarna kun je het meerdere keren oproepen en uitvoeren in je script*
```javascript
//De beschrijving van wat de funtie moet doen als deze aangeroepen wordt. Zelfde regels voor de naam van je function als bij je variabelen.
function congratulate() {
    console.log("Gefeliciteerd!");
}
//Het aanroepen van de hierboven gedeclareerde funtie. Deze kun je dus meerdere keren aanroepen op verschillende plekken in je script. 
congratulate();

```

###Functies met parameters:
*Hierbij zet je in de () van je function bijvoorbeeld name. Zo kun je dezelfde actie aanroepen maar een andere invulling er aan geven*
```javascript
//De funtie nu met een parameter ingevuld zoals name, deze zet je dan in je console log erbij waar je hem wilt hebben.
function congratulate(name) {
    console.log("Gefeliciteerd " + name + "!");
}
//Bij het aanroepen van deze functie moet je nu dus wel iets invullen tussen de haakjes, doe je dit niet dan krijg je undefined in je terminal. Onderstaand voorbeeld geeft nu "Gefeliciteerd Rianne!"
congratulate("Rianne");
```

###Return value:
*Hiermee kun je bijvoorbeeld een oppervlakte berekenen. Als de () wordt gedeclareerd noem je de informatie de parameters. Bij het oproepen noem je ze argumenten, hier geef een waarde op.*
```javascript
function area(width, length) {
    const outcome = width * length;
}
area(4, 6);
//Je kunt de outcome niet met console.log aanroepen buiten de funtie, net als bij een loop. Je moet hem als het waren terug geven, return. 
function area(width, length) {
    const outcome = width * length;
    return outcome;
}
area(4, 6);
//Dit is een beetje dubbel bij 1 variabel. Je kunt in dit geval gelijk de som teruggeven
function area(width, length) {
    return width * length;
}
area(4, 6);
//Om dit te loggen in de terminal zijn 2 opties.
//Zet de function in een console.log
console.log(area(4,6));
//Of je maakt een variabel aan.
const room1 = area(4, 6);
console.log(room1);
//Op deze manier kun je bijvoorbeeld een string maken met variables.
const room1 = area(4, 6);
const room2 = area(5, 7);
const room3 = area(8, 10);

const house1 = "De woonkamer is " + room1 + " m2, de keuken is " + room2 + " m2 en de slaapkamer is " + room3 + " m2."
console.log(house1);
```

###Regular vs Arrow Functions:
*Bovenstaande declaraties is de regular manier om een function te declareren. Een andere manier is de arrow function*
```javascript
//voorbeeld van een arrow funcion.
const area = (width, length) => width * length;
```
