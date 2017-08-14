# af-changelog

## I Test


------------

## I Produktion

### API v4.4.0 (I Test 2017-08-09)
* Stöd för sökning på flera kommuner. [#580](https://trello.com/c/692yUaTL/580)
* Omindexering av profiler tar bort avpublicerade profiler ur indexet. [#636](https://trello.com/c/2tvyHPaW/636)
* Sentry används för loggning av fel. [#606](https://trello.com/c/fmKJRGgJ/606)
* Förbättrad loggning av fel vid skickade av e-post. [#446](https://trello.com/c/8TefxoIt/446)
* Marknadsområden läggs in i databasen för användning för statistik. [#565](https://trello.com/c/dUd7E9aY/565)
* Bugfixar

### Sökgränssnitt v3.3.0 (I Test 2017-08-09)
* Man kan nu söka på flera kommuner samtidigt [#580](https://trello.com/c/692yUaTL/580)
* Räknaren som visar antal sökresultat är tillbaka [#630](https://trello.com/c/7hkaadAD/630)
* Man kan nu söka på hela mailadresser i IE11 [#551](https://trello.com/c/yA6tfEgS/551)
* Fixat ordningen/positionering av introtext på Profilsidan [#557](https://trello.com/c/uGQ4s6ft/557)

### Inmatningsgränssnitt v3.8.1 (I Test 2017-08-14)
* Tagit bort meddelandet på startsidan om att IE11 inte stöds

### Inmatningsgränssnitt v3.8.0 (I Test 2017-08-09)
* Vänsterställning av email- och lösenordsfält i RTL-språk [#604](https://trello.com/c/5NxcPUfs/604)
* Nollställning av årtal på yrkeserfarenhet [#601](https://trello.com/c/enMBIzp1/601)
* Rendering av radioknappar i IE11 [#618](https://trello.com/c/t7NhUeY6/618)
* Sök från lista i Yrkeserfarenheter och Kompetenser fixat i IE11 [#619](https://trello.com/c/Y36HV6o2/619)
* Indikator visas medan email skickas med CV [#396](https://trello.com/c/3iemMstK/396)
* Användaren loggas ut när sessionstiden gått ut, eller om token tas bort [#409](https://trello.com/c/5cfy34ix/409)
* Fixat bugg där man automatiskt slussades vidare direkt till Login-sidan istället för Start-sidan [#626](https://trello.com/c/jHuYTNh7/626)

### Sökgränssnitt v3.2.1 (I Test 2017-07-06, Produktionssatt 2017-08-07)
* Sökanvändare kan ladda ner arbetssökandes CV som PDF [#507](https://trello.com/c/dEdjmPs0/507)
* Inspectlet är inlaggt för användarvänlighets-studier [#605](https://trello.com/c/JcBc54wA/605)
* Nya underrubriker under "Sök" på Yrken och Karriärönskemål [#577](https://trello.com/c/aMRU2Feh/577)
* Tester för att säkerställa att Start-sidan fungerar som den ska efter införandet av arbetsgivarinloggning [#586](https://trello.com/c/Xq8cbm7Q/586)
* Flyttat upp länken till lathunden till headern i form av ett frågetecken [#599](https://trello.com/c/nFshC69K/599)
* Snyggat till 403-sidan [#593](https://trello.com/c/QBXhJ07m/593)

**OBS.** Alla ändringarna kom med i v3.2.0, men eftersom Sentry-scriptet inte kördes korrekt så rättades det till och versions-numret patchades upp. 

### Inmatningsgränssnitt v3.7.3 (I Test 2017-08-04, Produktionssatt 2017-08-07)
#### Hotfix
* Den nya "empty state"-designen i profilöversikten döljs för de sektioner där erfarenhet/språk/utbildning m.fl. saknas (så att det ser ut som innan). Detta tills vi fått ny copy och översättningar.

### Inmatningsgränssnitt v3.7.0 (I Test 2017-07-06, Produktionssatt 2017-08-07)
#### Features
* Notification bar tillaggd för att visa system- och felmeddelanden på Profilsidan [#589](https://trello.com/c/SknYfbFJ/589)
* Notifikation när CV mejlats visas på Profilsidan [#584](https://trello.com/c/9FzErK7e/584)
* Indikator (spinner) visas när man klickat på Skicka CV-knappen [#396](https://trello.com/c/3iemMstK/396)
* Empty state med hjälptexter tillaggda i Profilöversikten [#465](https://trello.com/c/MR9dJO4F/465)
* Publiceringspåminnelse visas för de som ej publicerat sina profiler än [#483](https://trello.com/c/9HY2Cn4P/483)

#### Bugfixar
* Hover på modalers stäng-knapp [#544](https://trello.com/c/1I18HRt0/544)
* Console-varning när man öppnade Personal Information fixad [#519](https://trello.com/c/MkLVMI3I/519)
* Fix av födelsedatums-inmatning i IE [#264](https://trello.com/c/E7UxyShB/264)
* Knapparna för Ladda ner och Skicka CV är disable:ade om man inte tickat i några bilagor [#545](https://trello.com/c/20PhzOMB/545)

### API v4.2.0 (I Test 2017-07-06, Produktionssatt 2017-08-07)
* Add coordination number to PDF-version of profile [#596](https://trello.com/c/zOjdEm8R/596)
* Make username case-insensitive and migrate all old users to have lowercased usernames [#174](https://trello.com/c/fki682vj/174)
* Add route to download PDF-version of profile for specific user [#507](https://trello.com/c/dEdjmPs0/507)
* Re-order search results based on number of matches [#530](https://trello.com/c/sjFrAoKv/530)

### API v4.3.0, Inmatningsgränssnitt v3.7.2 & Sökgränssnitt v3.2.4 (2017-07-14)
* Viktig [säkerhetsuppdatering av Node](https://nodejs.org/en/blog/vulnerability/july-2017-security-releases/).

### API v4.1.0 (2017-06-28)
* Fixat hasDegree när profiler om-indexeras [#418](https://trello.com/c/egP2S3K9/418) 
* Kollar roller från nya response-formatet från nya AF IDP [#403](https://trello.com/c/e1Kbff0U/403) 

### Sökgränssnitt v3.1.1 (I Test 2017-06-30, Produktionssatt 2017-06-30)
* Ny copy på startsidan [#583](https://trello.com/c/bP6qvEWt/583)
* Styling-fix på profilsidan, mer marginal på labels/ledtexterna [#550](https://trello.com/c/ndmTXbNA/550)

### Sökgränssnitt v3.1.0 (I Test 2017-06-28, Produktionssatt 2017-06-30)
* Arbetsgivarinloggning till Sök [#403](https://trello.com/c/e1Kbff0U/403)
* Sidtitel bytt till "Jobskills Sök" [#575](https://trello.com/c/5sdvOmxB/575)
* Robots.txt tillaggt för Infrastrukturskydd [#100](https://trello.com/c/6JarS5fo/100)
* Ny introtext på startsidan [#574](https://trello.com/c/Vldw2Uvp/574)
* Korrigerat positionering av info till arbetsgivare i IE11 [#562](https://trello.com/c/9yR6P58q/562)
* Logga ut-knappen visas bara när man är inloggad [#566](https://trello.com/c/bDXaWrdr/566)

### Inmatningsgränssnitt v3.6.2 (I Test 2017-06-28, Produktionssatt 2017-06-30)
* Robots.txt tillagt för Infrastrukturskydd [#100](https://trello.com/c/6JarS5fo/100)
* Ökad vidd på Publicera-knappens text för att få plats med Somaliska texten [#482](https://trello.com/c/otfbh7fk/482)
* Asterisk-markering på alla tvingande fält [#549](https://trello.com/c/JLDcxf3H/549)
* Valfri i rubriken på Nivå 3 på inmatningar [#537](https://trello.com/c/8HT6PG34/537)
* Email adressen tillaggd på sidan för Glömt lösenord [#212](https://trello.com/c/dFjBSiMu/212)
* Input-fälten är återställda till hur de var förrut [#494](https://trello.com/c/4gvzRKrV/494) & [#495](https://trello.com/c/W2o2vyRP/495)
* Email-validering sker i Skicka Profil [#547](https://trello.com/c/Z967IakC/547)
* Loggning i Frontend med Sentry [#487](https://trello.com/c/Tjfclv5L/487)
* Kommun kräver inte refresh längre för att uppdateras [#570](https://trello.com/c/ukoHGsAZ/570)
* Inspectlet tillaggt för användarstudier [#511](https://trello.com/c/VtO6luI3/511)

### Inmatningsgränssnitt v3.6.1 (2017-06-20)
* Hotfix: Hanterar `null`-värde i email när man loggar in med sociala medier, vilket förhindrade dessa användare från att redigera sin profil i v3.6.0 [#541](https://trello.com/c/XScwaRiA/541)

### Inmatningsgränssnitt v3.6.0 (2017-06-14)
* Årsinmatning återställt till endast ett inmatningsfält [#369](https://trello.com/c/xClCCuus/369)
* Google Analytics konfigurerat för att tracka fler events [#510](https://trello.com/c/gMqaLUxz/510)
* Användare loggas ut när deras Token/Cookie har gått ut [#505](https://trello.com/c/UjjNn0Bt/505)
* Man kan nu välja Grupp på Yrke, Karriärönskemål och Kompetenser [#527](https://trello.com/c/C17TIBE5/527)
* Nytt flöde för asyl och AT-UND inmatning [#469](https://trello.com/c/8KFYXngi/469)
* Studieinriktningar sorteras i alfabetisk ordning [#498](https://trello.com/c/WNmMmoQS/498)
* Man kan bara lägga till varje språk en gång bland Språkkunskaper [#476](https://trello.com/c/gQB4cxka/476)

### Sökgränssnitt v3.0.5 (I Test & Prod 2017-06-22)
* Labels tillagda för personuppgifter på profiler [#550](https://trello.com/c/ndmTXbNA/550)
* Uppdaterat till lathund v1.2. Öppnas i ny flik när man klickar på den. [#528](https://trello.com/c/ben0J3OM/528)
* (Valfri) i rubriken på nivå 3 av sök på Yrke och Karriärönskemål [#560](https://trello.com/c/jPtUrsr0/560) 

### Sökgränssnitt v3.0.4 (I Test 2017-06-21, I Prod 2017-06-22)
* Laddat upp senaste versionen av lathunden, och fixat länken från Profil-sidan [#528](https://trello.com/c/ben0J3OM/528)

### Sökgränssnitt v3.0.3 (I Test 2017-06-20, I Prod 2017-06-22)
* Lathund tillaggd i footern [#528](https://trello.com/c/ben0J3OM/528)
* Rättat ordningen på infon för arbetsförmedlare/arbetsgivare [#535](https://trello.com/c/XD3Hlv42/535)

### Sökgränssnitt v3.0.2 (I Test 2017-06-16, I Prod 2017-06-20)
* Råkade hoppa direkt till v3.0.2 ist för v3.0.1. så versionsnumret är korrekt angivet här, det finns ingen v3.0.1.
* Lagt till kontroll för när namn saknas hos användare i sökresultat så att det ska stå "Ej angivet" istället för "null null".

### Sökgränssnitt v3.0.0 (I Test 2017-06-15, I Prod 2017-06-20)
#### Breaking Changes
* Visa uppfyllda och ej uppfyllda kriterier i sökresultaten [#463](https://trello.com/c/xo2Tf1Em/463). Kräver API v4.0.0

#### Features & Bug fixes
* Hantering av tom data [#523](https://trello.com/c/cOYDOw7h/523)
* Namnet på personen sätts på tabben när man öppnat ny tab med profil [#521](https://trello.com/c/6V3mLz1Y/521)
* Utloggning leder nu till `/` istället för att loopa nonstop [#444](https://trello.com/c/wxphWdt2/444)
* Feedback-formulär tillaggt [#515](https://trello.com/c/poNAHHGX/515)
* Sökningar fördröjda med 1 sekund för att förhindra "sönderhackade" sökningar [#449](https://trello.com/c/MYSiIDed/449)
* Info om anställning av Asylsökande, AT-UND m.m. tillagt på Profil-sidan [#479](https://trello.com/c/kQ7xs0LI/479)

### API v4.0.0 (I Test 2017-06-15, I Prod 2017-06-20)
Now admin search results return not just names of filters that were met, but instead all filters with a flag isMatch [#463](https://trello.com/c/xo2Tf1Em/463)

### API v3.1.4 (I Test 2017-06-09, I Prod 2017-06-20)
* Fixar filtrering på Examen i Sökgränssnittet [#418](https://trello.com/c/egP2S3K9/418)

### API v3.1.3 (I Test 2017-05-24, I Prod 2017-06-20)
* Visar/Skickar korrekt informationstext från Utbildning och Utbildningsnivå [#306](https://trello.com/c/0EYM7Akw/306)

### Inmatningsgränssnitt v3.5.1 (I Test 2017-05-24, I Prod 2017-06-20)
* Tvingande fält är tillagda i Personuppgifter och markerade med röd asterisk [#450](https://trello.com/c/eOERx5RI/450)
* Icke-Latinska tecken kan inte längre sparas i Personuppgifter när man kör Wizard [#478](https://trello.com/c/HSyDle9x/478)
* Google Analytics är tillagt, med tracking på sidbyten (stöd finns även för att tracka clicks och andra events) [#370](https://trello.com/c/MmF5A0oD/370)

### Inmatningsgränssnitt v3.5.0 (I Test 2017-05-24, I Prod 2017-06-20)
#### Features
* Karriärguiden visar text på utbildningsinriktning istället för utbildningsnivå när det finns [#306](https://trello.com/c/0EYM7Akw/306)
* Prestandaoptimeringar av frontend [#458](https://trello.com/c/xupNhGkz/458)
* Ny design av hjälprutor [#485](https://trello.com/c/s5RXn9Tf/485)
* När användaren väljer "Välj i lista" så öppnas första listan som default [#470](https://trello.com/c/D4pQXBsb/470)
* Nytt inmatningsflöde för Asylstatus och AT-UND [#469](https://trello.com/c/8KFYXngi/469)

#### Buggfixar
* Profil-text på Somaliska fixad [#482](https://trello.com/c/otfbh7fk/482)
* Samt mindre designfixar [#486](https://trello.com/c/HhCR2SHr/486), [#480](https://trello.com/c/zWCuj5dx/480), [#459](https://trello.com/c/kPzPLoaZ/459) och [#481](https://trello.com/c/DIbcl4F3/481)

### Sökgränssnitt v2.0.3 (2017-05-23)
* Anpassat sök-gränssnittet för att fungera med olika skärmstorlekar [#454](https://trello.com/c/wymUdXKa/454)

### Inmatningsgränssnitt v3.4.0 (2017-05-23)
#### Buggfixar
* Tagit bort den extra Språk-labeln i Inställningar [456](https://trello.com/c/RowNAgQo/456)
* Hela korten i karriärguiden är klickbara [#455](https://trello.com/c/JxQznRUI/455)
* Grafiska buggar fixade i språkvalsraden [#453](https://trello.com/c/yVW1BeuU/453)

#### Features
* Inmatning av födelsedatum är uppdelat i 3 fält  (år, månad och dag) [#457](https://trello.com/c/aVDLsh6p/457)
* I "Välj från lista"-Inmatningen av Yrkeserfarenhet och Karriärönskemål dyker en nivå upp i taget [#451](https://trello.com/c/9rX3zlwj/451)
* Inmatning tillåter bara latinska tecken [#372](https://trello.com/c/01UP4uta/372)

### API v3.1.2 (2017-05-18)
Fixade översättningssträngar i PDF-versionen av profilen [#460](https://trello.com/c/oZ83bX7k/460)

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
* Man kan komma till Sök från AF:s sidor (Vis) utan att behöva logga in [#324](https://trello.com/c/Se2p6VN8/324-komma-till-sok-fran-af-s-sidor)

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
