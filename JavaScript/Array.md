#Arrays:
*Een array is een data type dat een lijst maakt, deze wordt vaak gebruikt als de lijst allemaal dezelfde waarde heeft. Is geen must maar wel hoe het in de praktijk gebruikt wordt.*

**CRUD: C= create, R= read, U= update, D= delete**
###Create:
*Een array maak je door een const aan te maken met de waarde tussen blokhaken. Zorg altijd dat er een comma tussen de verschillende arrays staat.*
```javascript
//Maak een array aan:
const years  = [2019, 2020, 2021, 2022];

```

###Read:
*Hoe lees, toon je een array in de terminal. En hoe kun je enkele waarde van de array loggen in de terminal.*
```javascript
//laat de volledige array zien
console.log(years);
//laar de volledige array zien zonder de [] er omheen
console.log(...years);
//laat de laatste waarde in bovenstaand voorbeeld zien.
console.log(years[3]);
//of
const nextYear = years[3];
console.log(nextYear);

//Veranderen de waarde in je array en wil je altijd bijvoorbeeld de laaste waarden laten zien. 
// deze past zich dan steeds aan ookal komen er nieuwe waardes bij.
const futureYear = years[years.length - 1];
console.log(futureYear);
```

###Update:

*Hoe pas je waardes in een array aan. Let er op dat je bij een const alleen enkele invoer kunt aanpassen. Bij een let kun je de gehele waarde aanpassen op een later moment.*
```javascript
//Het aanpassen van een bepaalde waarde in de array
years[3] = "2023";
//Als je let hebt gekozen als variable dan kun je de gehele array zo aanpassen. 
// Alle waardes worden dan overschreven, ook als je meer of minder waardes in je array zet.
years = [2018, 2017, 2016, 2017];
//Extra waarde toevoegen aan de bestaande array aan het eind van de array.
years.push(2025);
//Extra waarde toevoegen op specifieke plek. eerste cijver is welke plek in de array 0 is 1e waarde. 
// Tweede cijfer is welke waarde je wilt verwijderen. Derde input is wat je wilt toevoegen.
years.splice(0, 0, 2018); //zet dus 2018 voor aan de array zonder de andere te verwijderen.
```

###Delete:

*Het verwijderen van waarde in je array zonder de oiginele variable aan te passen.*
```javascript
//De laatste waarde in je array verwijderen.
years.pop();
//De eerste waarde in je array verwijderen.
years.shift();
//Een waarde verwijderen op een andere positie.
years.splice(1, 1); //Haalt de waarde op positie 1 weg. Geen 3e argument invullen als je niks wil toevoegen.
years.splice(1, 2); //Vanaf waarde 1 verwijdert hij er 2
```

