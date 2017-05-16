# af-changelog

## På test

------------

## I produktion

### Inmatningsgränssnitt v3.3.2 (2017-05-16)
* Fixat så att språk uppdateras när man väljer ett annat på Startsidan eller i Inställningar [#441]
* Man kan ändra år, examen och inriktning i Redigerings-läget av Utbildningar [#312]

### API v3.1.0 (2017-05-16)
#### Breaking
* Vi gör queries direkt mot CMS:et [#432]

#### Förbättringar
* Uppdaterat Utbildnings-queryn [#306]
* Tagit bort 'deprecated fields' [#407]
* Sätter en kortare expiry på token [#409]
* Tillåter API:et att läsa krävda SAML certifikat genom environment variabler
* Docker-compose är mer konfigurerbar

### Sökgränsnitt v2.0.2 (2017-05-15)
* Paginering: När det är många sidor görs radbyte för att förhindra att sid-knapparna hamnar utanför kanten [#373]
* Positionerat sidbytesknapparna längst ner [#373]
* Årsparametrar visas nu i sökkriterier [#416]
* Förslag på sökresultat visas nu när man söker ort [#415]

### Sökgränsnitt v2.0.1 (2017-05-08)

* Vi korrigerade så att antal träffar per sida fungerar korrekt med paginering. 
* Det går att välja mellan att visa 10, 25 eller 50 resultat per sida, och vi hämtar bara så många resultat åt gången för att minska belastningen på API:et.
* Antal år och examen visas nu bara på relevant utbildningsnivå.

### Inmatningsgränssnitt v3.3.1 (2017-05-12)
* Fixade så att Education fungerar igen. [#436]
* Låst ner våra dependencies, så att vi alltid använder samma i Produktion, Test och CI.

### Inmatningsgränssnitt v3.3.0 (2017-05-09)
* Varje info-ruta i Karriärguiden visas bara en gång. [#399]
* Radioknapparna fixade i Personuppgifter-modalen så att man kan klicka Nej på AT-UND, Asyl m.fl. [#347]
* Antal år är tvingat i Yrkeserfarenhet och kompetenser [#397]
* Wizard kan startas om ifrån Inställningar-sidan. [#402]

### Inmatningsgränssnitt v3.2.0 (2017-05-05)
* Inmatning av namn och telefonnummer tillåter nu enbart latinska tecken
* Det är nu obligatoriskt att ange antal år för yrkeserfarenhet / kompetens
* Man kan ny fylla i att man har examen vid val av utbildningsnivå: gymnasium

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
