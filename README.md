# af-changelog

## På test

### Sökgränsnitt v2.0.1 (2017-05-08)

* Vi korrigerade så att antal träffar per sida fungerar korrekt med paginering. 
* Det går att välja mellan att visa 10, 25 eller 50 resultat per sida, och vi hämtar bara så många resultat åt gången för att minska belastningen på API:et.
* Antal år och examen visas nu bara på relevant utbildningsnivå.

### Inmatningsgränssnitt v3.2.0 (2017-05-05)

* Inmatning av namn och telefonnummer tillåter nu enbart latinska tecken
* Det är nu obligatoriskt att ange antal år för yrkeserfarenhet / kompetens
* Man kan ny fylla i att man har examen vid val av utbildningsnivå: gymnasium

------------

## I produktion

### API v.2.0.1 (2017-05-04)
#### Buggar
* Fixar sökning på födelsedatum, eller början av ett.

### Sökgränssnitt v2.0.0 (2017-05-04)
#### Features
* Man kan nu söka på samordningsnummer, eller början av ett.
* Man kan söka på födelsedatum, eller början av ett.
* Informationskortet visar om man har en examen på sin utbildning, samt antal år per utbildning.
* Sök-användare kan se totala antalet träffar på sin sökning, högst upp på sidan.
* Sökning på Ort, Kön, Samordningsnummer och Födelsedatum visar s.k. "Taggar", de blåa textfälten som visar vad man sökt på.

### API v2.0.0 (2017-05-04)
**Breaking changes**
API:et förväntar sig en ny struktur på Sök-gränssnittets förfrågningar, därför syns inte svaren korrekt.

#### Features
* Stöd finns för skip och limit, för att kunna begränsa antalet sökresultat man vill hämta vid varje sökning. Detta för att inte hämta onödigt mycket data.
* Totala antalet sökresultat skickas nu med som en siffra vid sökning.
* Verifierings-mail tillagt för Somaliska.

#### Buggar
* API:et sparar en tidsstämpel på när man senast loggat in, detta för att kunna automatiskt avpublicera inaktiva användares profiler.

### Inmatningsgränssnitt v3.1.1 (2017-05-04)
#### Buggar
* Tagit bort tangentbordet vid inmatning i Education och andra inmatningsfält.
* Lagt till email adress på /verify-email sidan.

### API v1.10.0 (2017-05-02)

Ändrat format för samordningsnummer. Formen är nu YYYYMMDDXXXX. Detta möjliggör sökning oavsett hur siffran har fyllts i.

### Sökgränssnitt v1.3.0 (2017-05-02)

Sökning på ort möjlig.

### API v1.9.0 (2017-04-30)

Omindexering för att sökning ska fungera på e-postadress.
