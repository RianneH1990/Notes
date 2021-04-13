#Objects
*Een object is een lijst waarvan de waarde gedefineerd word met een key. Hierdoor kun je makkelijker zien welke waarde er in je object staat. Daarom wordt object in de regel gebruikt om een lijst te maken met verschillende soorten waarde.*

**CRUD: C= create, R= read, U= update, D= delete**
###Create:
*Een object maak je door een const aan te maken met de waarde tussen snorhaken {}. Zorg altijd dat er een comma tussen de verschillende objecten staat. Je kunt ook elke object op een nieuwe regel zetten, zodat het overzichtelijker is. Hier zet je tussen de key en de value een :. Ook kun je de key tussen aanhalings tekens plaatsen mocht je bijvoorbeeld streepjes in de naam van je key willen gebruiken.*
```javascript
//Maak een object aan:
const personal  = {
    name: "Rianne",
    age: 30,
    "d-o-b": new Date(Date.UTC(1990, 03, 15)),
    city: "Utrecht",
}
```

###Read:
*Hoe lees, toon je een object in de terminal. En hoe kun je enkele waarde van de objecten loggen in de terminal.*
```javascript
//laat de volledige objects zien
console.log(personal);
//laat de specfieke waarde zien. Let op de key wordt niet meegelogd
console.log(personal.name);
//met bijzondere notatie "key".
console.log(personal["d-o-b"]);
//of
const myName = personal.name;
console.log(myName);
```

###Update:

*Hoe pas je waardes in een object aan. Let er op dat je bij een const alleen enkele invoer kunt aanpassen. Bij een let kun je de gehele waarde aanpassen op een later moment.*
```javascript
//Het aanpassen van een bepaalde waarde in de object
personal.age = 31;
//Als je let hebt gekozen als variable dan kun je de gehele array zo aanpassen. 
// Alle waardes worden dan overschreven, ook als je meer of minder waardes in je array zet.
personal {name: Robbert, age: 33, dob: new Date(Date.UTC(1987, 10, 20)), city: Vlaardingen};
//Extra waarde toevoegen aan de bestaand object aan het eind.
personal.job = "student";
```

###Delete:
*een key verwijderen uit het object.*
```javascript
delete personal.age;
```

