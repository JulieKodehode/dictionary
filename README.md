# Oversikt i JavaScript
## Innholdsfortegnelse

- [Symboler](#Symboler)
- [Datatyper](#Datatyper)
  - [Primitive datatyper](#Primitive-datatyer)
  - [Ikke-primitive datatyper](#Ikke-primitive-datatyer)
- [Variabler](#Variabler)
- [Funksjoner](#Funksjoner)
- [DOM Manipulasjon](#DOM-Manipulasjon)
- [Hendelseslytter](#Hendelseslytter)

## Symboler (Symbols)

- `[]` – Braketter (square brackets). Brukes til å definere arrays (lister) og for å hente ut elementer fra arrays eller objekter.

Eksempel:
```javascript
let liste = [1, 2, 3];
console.log(liste[0]); // 1
```

- `()` – Parenteser (parentheses). Brukes til å definere parametere ved funksjonserklæring og til å sende inn argumenter ved funksjonskall.

Eksempel:
```javascript
function hils(navn) {
  console.log("Hei, " + navn);
}
hils("Ola");
```

- `{}` – Krøllparenteser (curly brackets). Brukes for å definere kodeblokker (i funksjoner, if-setninger osv.) og til å definere objekter.

Eksempel:
```javascript
let person = {
  navn: "Ola",
  alder: 25
};
```

- `""` – Dobbelte hermetegn (double quotes). Brukes til å lage tekststrenger. Du kan også bruke `'` (enkle hermetegn) med samme resultat, eller `` (backticks) for template literals.

Eksempel:
```javascript
let tekst = "Hei verden";
```

- `=` – Tildelingsoperator (assignment operator). Brukes til å tilordne en verdi til en variabel.

Eksempel:
```javascript
let alder = 30;
```

## Datatyper (Data Types)

### Primitive datatyper (Primitive Data Types)

- `number` – Et tall, f.eks. 42 eller 3.14.

Eksempel:
```javascript
let tall = 10;
```

- `string` – En tekststreng, f.eks. "Hei verden".

Eksempel:
```javascript
let melding = "God morgen";
```

- `boolean` – Sant eller usant, `true` eller `false`.

Eksempel:
```javascript
let erLoggetInn = true;
```

- `undefined` – En verdi som ikke er definert eller ikke er tildelt.

Eksempel:
```javascript
let x;
console.log(x); // undefined
```

- `NaN` – Står for "Not a Number". Oppstår når du forsøker å gjøre matematikk på noe som ikke er et tall.

Eksempel:
```javascript
let resultat = "tekst" / 2;
console.log(resultat); // NaN
```

### Ikke-primitive datatyper (Non-Primitive Data Types)

- `array` – En liste med verdier, som kan inneholde ulike datatyper.

Eksempel:
```javascript
let blandet = [1, "tekst", true];
```

- `object` – En samling med nøkkel-verdi-par.

Eksempel:
```javascript
let bok = {
  tittel: "Min bok",
  sider: 200
};
```

## Variabler (Variables)

- `let` – Deklarerer en variabel som kan endres. Gyldig innenfor blokken den er definert i.

Eksempel:
```javascript
let navn = "Per";
navn = "Kari";
```

- `const` – Deklarerer en konstant verdi som ikke kan reassignes. NB: For arrays og objekter kan innholdet fortsatt endres.

Eksempel:
```javascript
const PI = 3.14;
```

## Funksjoner (Functions)

- `function` – Nøkkelord som brukes til å erklære en funksjon.

- `function navnPaFunksjon() {}` – Funksjonserklæring.

- `()` – Brukes til å definere eller sende inn parametere/argumenter.

- `{}` – Inneholder funksjonens logikk, altså hva som skal skje når funksjonen kjører.

Eksempel:
```javascript
function siHei(navn) {
  console.log("Hei, " + navn);
}
siHei("Nora");
```

## DOM Manipulasjon (DOM Manipulation) (Document Object Model Manipulation)

- `document` – Refererer til HTML-dokumentet i nettleseren.

- `getElementById()` – En metode for å hente et element med et spesifikt `id`-navn.

Eksempel:
```javascript
document.getElementById("button");
```

- `querySelector()` – En metode for å hente det første elementet som matcher en CSS-selektor (tag, klasse eller ID).

Eksempel:
```javascript
document.querySelector("#button");
```

- `.textContent` – Brukes til å lese eller sette tekstinnholdet i et element.

Eksempel:
```javascript
userName.textContent = "Julie";
```

- `.style` – Brukes til å legge til inline CSS-stil direkte på et element.

- `.style.width` – Brukes til å sette bredden direkte på et element via inline styling.

Eksempel:
```javascript
image.style.width = "100%";
```

- `.classList` – Refererer til en liste over alle klassene som er knyttet til et element.

- `.classList.add` – Legger til en klasse til elementets classList.

Eksempel:
```javascript
knapp.classList.add("aktiv");
```

## Hendelseslytter (Event Listener)

- `.addEventListener()` – En metode som brukes for å lytte etter hendelser på HTML-elementer.

Første parameter: navnet på hendelsen, f.eks. "click".

Andre parameter: en callback-funksjon som skal kjøres når hendelsen skjer.

Eksempel:
```javascript
let knapp = document.querySelector("button");
knapp.addEventListener("click", function () {
  console.log("Knappen ble klikket!");
});
```

