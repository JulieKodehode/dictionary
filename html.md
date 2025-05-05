# Oversikt i HTML

* [Grunnstruktur](#Grunnstruktur)
* [Semantiske elementer](#Semantiske-elementer)
* [Attributter](#Attributter)
* [Tekst og innhold](#Tekst-og-innhold)
* [Skjemaelementer](#Skjemaelementer)
* [Kommentarer](#Kommentarer-i-html)

## Grunnstruktur

HTML-dokumenter starter med en deklarasjon og struktureres med hovedtaggene `<html>`, `<head>` og `<body>`:

* `<!DOCTYPE html>`: Forteller nettleseren at dette er et HTML5-dokument.
* `<html>`: Rotelementet som inneholder hele HTML-strukturen.
* `<head>`: Inneholder metadata, som tittel, stilark og script.
* `<body>`: Inneholder alt innholdet som vises på nettsiden.

Eksempel:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Min side</title>
  </head>
  <body>
    <!-- Innhold vises her -->
  </body>
</html>
```

## Semantiske elementer

Semantiske elementer gir mening til innholdet og gjør det lettere å forstå strukturen for både utviklere og søkemotorer:

* `<header>`: Representerer toppen av en side eller seksjon.
* `<nav>`: Inneholder navigasjonslenker.
* `<main>`: Hovedinnholdet på siden.
* `<section>`: En tematisk seksjon av innhold.
* `<article>`: Et selvstendig stykke innhold, som en bloggpost eller nyhetsartikkel.
* `<aside>`: Innhold som er perifert relatert til hovedinnholdet, f.eks. en sideboks.
* `<footer>`: Bunntekst for en side eller seksjon.

Eksempel:

```html
<main>
  <article>
    <h2>Nyhet</h2>
    <p>Dette er en artikkel.</p>
  </article>
</main>
```

## Attributter

Attributter gir ekstra informasjon til HTML-elementer:

* `id`: En unik identifikator for et element.
* `class`: Brukes til å gruppere elementer for styling eller scripting.
* `src`: Kilde for medier (f.eks. bilder, script).
* `alt`: Alternativ tekst for bilder, viktig for tilgjengelighet.
* `href`: Lenkeadresse i `<a>`-elementer.
* `target`: Definerer hvor en lenke skal åpnes, f.eks. `_blank` for ny fane.

Eksempel:

```html
<a href="https://eksempel.no" target="_blank">Åpne i ny fane</a>
<img src="bilde.jpg" alt="Beskrivende tekst">
```

## Tekst og innhold

Disse taggene brukes til å strukturere og vise tekstlig innhold:

* `<h1>`–`<h6>`: Overskrifter, der `<h1>` er størst og viktigst.
* `<p>`: Avsnitt
* `<a href="">`: Lenker
* `<img src="" alt="">`: Bilder
* `<ul>`, `<ol>`, `<li>`: Lister (henholdsvis uordnet og ordnet)

Eksempel:

```html
<h1>Velkommen</h1>
<p>Dette er et avsnitt.</p>
<a href="https://eksempel.no">Besøk nettsiden</a>
```

## Skjemaelementer

Skjema brukes til å samle inn data fra brukeren:

* `<form>`: Skjemakonteiner
* `<input>`: Inndatafelt med ulike typer (tekst, e-post, passord, etc.)
* `<label>`: Knytter tekst til et spesifikt felt
* `<textarea>`: Flertlinjet tekstfelt
* `<select>` og `<option>`: Nedtrekksmeny

Eksempel:

```html
<form>
  <label for="navn">Navn:</label>
  <input type="text" id="navn" name="navn">
  <input type="submit" value="Send">
</form>
```

## Kommentarer i HTML

Kommentarer brukes for å forklare koden, og vises ikke i nettleseren:

```html
<!-- Dette er en kommentar -->
```
