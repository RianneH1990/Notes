#Loops

##for loop
*standaard for loop*
```javascript
//dit is de standaard formule voor een for loop
for (let i = 0; i < 10; i++) {
    console.log(i);
}
// alles in de loop in aan te passen, het eerste stuk is waar de loop moet beginnen 0 is beginnen bij het 1. 
// Maar dit kan ook 5 of 100 zijn, zolang het maar onder het cyfer wat in het 2e deel wordt gebruikt. 
// In het 2e deel kun je aangeven tot waar de loop moet lopen. dus hier stopt de loop als het groter wordt dan 10. 
// Het 3e stuk is de som die de loop maakt, hier is het plus 1 maar dit kan ook plus 2 worden.
```

*Arrays in loops*
```javascript
//Je kunt de array aanspreken in een loop, hierbij kun je de waarde van de array ook aanpassen. 
// Dus in onderstaand voorbeeld wordt elke waarde in de array aangesproken en wordt er "je" aan toegevoegd. Maar je kunt ook sommen maken.

const names = ["Henk", "Piet", "Fred", "Joop"];
console.log(names);
for (i = 0; i < names.length; i++) {
    names[i] = names[i] + "je";
}
console.log(names);
```

