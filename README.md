# af-changelog

## Sökgränssnitt v2.0.0 (2017-05-04)
### Features
* Man kan nu söka på samordningsnummer, eller början av ett.
* Man kan söka på födelsedatum, eller början av ett.
* Informationskortet visar om man har en examen på sin utbildning, samt antal år per utbildning.
* Sök-användare kan se totala antalet träffar på sin sökning, högst upp på sidan.
* Sökning på Ort, Kön, Samordningsnummer och Födelsedatum visar s.k. "Taggar", de blåa textfälten som visar vad man sökt på.

## API v2.0.0 (2017-05-04)
**Breaking changes**
API:et förväntar sig en ny struktur på Sök-gränssnittets förfrågningar, därför syns inte svaren korrekt.

### Features
* Stöd finns för skip och limit, för att kunna begränsa antalet sökresultat man vill hämta vid varje sökning. Detta för att inte hämta onödigt mycket data.
* Totala antalet sökresultat skickas nu med som en siffra vid sökning.
* Verifierings-mail tillagt för Somaliska.

### Buggar
* API:et sparar en tidsstämpel på när man senast loggat in, detta för att kunna automatiskt avpublicera inaktiva användares profiler.

## Inmatningsgränssnitt v3.1.1 (2017-05-04)
### Buggar
* Tagit bort tangentbordet vid inmatning i Education och andra inmatningsfält.
* Lagt till email adress på /verify-email sidan.

## API v1.10.0 (2017-05-02)

Ändrat format för samordningsnummer. Formen är nu YYYYMMDDXXXX. Detta möjliggör sökning oavsett hur siffran har fyllts i.

## Sökgränssnitt v1.3.0 (2017-05-02)

Sökning på ort möjlig.

## API v1.9.0 (2017-04-30)

Omindexering för att sökning ska fungera på e-postadress.
