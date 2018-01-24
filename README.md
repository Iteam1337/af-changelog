# af-changelog

## I Test

### API v6.1.1 (I test 2018-01-23)
- Fix för att hantera .some( som kastas av api:et vid sökningar av flera erfarenheter

### API v6.1.0 (I test 2018-01-23)
#### Breaking changes
- Indexera bara de profiler som finns i den urk:version som används
#### Fixes
- Sorterar sökindexen efter flest träffar + flest år

### API v6.0.0 (I test 2018-01-23)
#### Breaking changes
- Anonymiserad databas
- CORS-förändringar
- Personuppgifter indexeras inte i elasticsearch

### Sökgränssnitt v5.0.2 (I test 2018-01-23)
- Styling-fixar i IE11 [sprintboard #344](https://trello.com/c/Mc4F7cZ8/344) och Profil-sidan [sprintboard #303](https://trello.com/c/dBe1tWGO/303)
- Klickar man bort en områdes-tagg så avmarkeras den även i Områdes-fliken [Jobb #1104](https://trello.com/c/WDgkotW2/1104)
- Fixat till bakgrundsfärgerna [Jobb #1115](https://trello.com/c/L8WyR3Tq/1115)
- Om man återställer alla sökkriterier så ser det ut som innan man gjort en sökning, dvs den matchar inte på _alla_ kandidater [Jobb #1095](https://trello.com/c/rml0OuSa/1095)
- Fritextsöket innuti Yrke-, Område- och Kompetens-tabbarna fungerar igen [Jobb #1106](https://trello.com/c/FmGUObeW/1106) och [sprintboard #363](https://trello.com/c/GD92dzGo/363)
- När man byter mellan sidorna hamnar man nu högst upp på sidan [Jobb #1091](https://trello.com/c/Z6XAA7Vz/1091) och [Jobb #1094](https://trello.com/c/DaLngiiD/1094)
- Feedback-formuläret är nu på Svenska [Jobb #1098](https://trello.com/c/oDAUDJA2/1098) och länktexten är ändrad [Jobb #1097](https://trello.com/c/d2GPbKVc/1097)
- Tips på liknande sökkriterier har döljts tillfälligt [#1107](https://trello.com/c/AjVYhDrs/1107)
- Erfarenhetsmätaren på Yrke & Kompetenser matchar mellan fritext- och tabbarna [Jobb #1100](https://trello.com/c/Mxj0NdHi/1100)
- Erfarenhetsmätaren är inkluderande på år [Jobb #1099](https://trello.com/c/6KzIYFlx/1099)
- Områden är ikryssade i Områdes-fliken efter att man valt i fritext-söket [#1105](https://trello.com/c/UrQaKNt3/1105)
- Pagineringsvalet återställs vid ny sökning [sprintboard #338](https://trello.com/c/nvIRt0iC/338)

### Sökgränssnitt v5.0.1 (I test 2018-01-18)
- Fixat felaktig styling där vissa äldre webbläsare inte visade sidorna som en kolumn (med headern överst, sen body, följt av footern nederst) - allt låg i sidled (row).
- Lagt till unika keys för alla tags (för att förhindra renderings-problem och console-varningar).

### Sökgränssnitt v5.0.0 (I test 2018-01-18)
Det nya söket [#927](https://trello.com/c/XwUGPKSr/927) och en massa andra Trello-kort.

### Inmatningsgränssnitt v.4.0.7 (I test 2018-01-23)
- Lagt tillbaka alla länkarna till Sökgränssnittet från Start-sidan (i headern, dess sidomeny som visas i mobil, i bodyn, och i footern), samt mindre styling-fixar i RTL-språk för dessa länkar [#328](https://trello.com/c/YDDZZtNU/328)

### Inmatningsgränssnitt v4.0.6 (I test 2018-01-16)
- Användarspråken visas efter att man loggat ut [#1068](https://trello.com/c/lt0vgJVa/1068)
- Arbetsförmedlingen- och Jobskills-loggorna klipps inte av i mobil [#1068](https://trello.com/c/lt0vgJVa/1068)
- Kosmetisk fix av startsidans inforuta [#1069](https://trello.com/c/mkvoJNCR/1069)

### Inmatningsgränssnitt v4.0.5 (I test 2018-01-15)
- Fixat så att sidomenyn ine blockerar halva skärmen i IE11 [#1068](https://trello.com/c/lt0vgJVa/1068)
- Fixat så att nyhetssidan inte bara visas ihopträngd i övre vänstra hörnet i IE11 [#1068](https://trello.com/c/lt0vgJVa/1068)
- Tagit bort länken till `Om Jobskills`-sidan som inte finns än
- Mindre styling-fixar i RTL-språk

### Sökgränssnitt v4.0.7 (I test 2017-11-23)
(_v.4.0.6 bumpningen failade, innehåller samma ändringar som denna version_)
- Tagit bort Beta-information för handläggare [#1033](https://trello.com/c/QOeXVHFL/1033)
- Uppdaterat copy på `/arbetsgivarinformation`(lagt till ingress och ändrat lite styling) 

### API-import v1.0.0 (I test 2017-10-26)
- [#380 yrkeskompetenser](https://trello.com/c/Hq2V30el/380-att-ta-med-yrkeskompetenser-under-yrkesgrupper-xl-del-av-390-i-ci-develop)
- Hantera konflikter där `ID` inte är unikt i postgres

------------

## I Produktion

### Inmatningsgränssnitt v4.0.4 (I test 2018-01-15, Produktionssatt 2018-01-15)
(_v.4.0.3 bumpningen failade, innehåller samma ändringar som denna version_)
- Ny design på startsidan och headern.
- Tagit bort Sentry för exception-hantering.


### Sökgränssnitt v4.0.5 (I test 2017-11-17, Produktionssatt 2017-11-17)
* Ändrad logik för när vilken hjälptext visas på `/profil`-sidan:
  * Har man AT-UND -> hjälptexten för `DET HÄR ÄR EN ASYLSÖKANDE SOM FÅR ARBETA`
  * Har man Uppehållstillstånd -> Hjälptexten om `DET HÄR ÄR EN NYANLÄND SOM FÅR ARBETA`
  * Har man inte AT-UND -> Hjälptexten om `DET HÄR ÄR EN ASYLSÖKANDE SOM INTE FÅR ARBETA ÄN`

* Uppdaterad copy för ovanstående hjälptexter
* Tagit-bort modalen som länken öppnade och länkar istället till `/arbetsgivarinformation`-sidan

### Sökgränssnitt v4.0.4 (I test 2017-11-17, Produktionssatt 2017-11-17)
- Korrigerat copy och lagt till en `tillbaka`-knapp på `/arbetsgivarinformation`-sidan

### Sökgränssnitt v4.0.3 (I test 2017-11-16, Produktionssatt 2017-11-17)
- Arbetsgivare kan inte söka på samordningsnummer och inte heller se dem på en kandidats profilsida [#1017](https://trello.com/c/RKcd79bg/1017)
- Ny informationssida för arbetsgivare på `/arbetsgivarinformation` [#1024](https://trello.com/c/E1wqLdJL/1024)
- Beta-info på söksidan och i header [#1023](https://trello.com/c/ILsFi39z/1023)
- Sökrutor för fritext har förstoringsglas istället för dropdown-design [#1022](https://trello.com/c/c0T1F9ta/1022)
- Hjälp-info om utbildningar i Utbildningar-sökboxen [#1021](https://trello.com/c/6eQ7M06t/1021)
- Tagit bort automatisk redirect från start-sidan till inlogget, man måste klicka på `Logga in` nu [#1020](https://trello.com/c/0xuEhMUA/1020)
- Ny profilsida [#1019](https://trello.com/c/CScudCTO/1019)
- Klickar man på en sök-kandidat i resultat-listan så öppnas det i samma flik, med en `Tillbaka`-knapp upptill som går tillbaka till där man senast var i resultatlistan (samma kandidater, sökning osv)

### API v5.1.0 (Produktionssatt ca 2017-11-09)
- Använd mailkön för email
- Funktionalitet för varningar och avpublicering av inaktiva användare.

### API v5.0.1 (I test 2017-10-26, Produktionssatt 2017-11-09)
- [#380 yrkeskompetenser](https://trello.com/c/Hq2V30el/380-att-ta-med-yrkeskompetenser-under-yrkesgrupper-xl-del-av-390-i-ci-develop)
- Versionering av urk-version
- Omskrivna SQL-frågor

Denna release ändrar strukturen för taxonomin.
Vi använder inte längre taxonomy_work och/eller taxonomy_competences. De är sammanslagna till `taxonomy`.

### Inmatningsgränssnitt v4.0.2 (I test 2017-10-27, Produktionssatt 2017-10-27)
- Fixar ett fel där fälten för `Studieinriktning` och `År` var tomma när redigeringsläget för utbildningar öppnades. Det gick inte heller att ändra utbildning och antal år - nu är det fixat. [#914](https://trello.com/c/PEgDeW0h/914)

### Inmatningsgränssnitt v4.0.0 (I test 2017-10-26, Produktionssatt 2017-10-27)
- Hanterar den nya taxonomi-strukturen, med Yrkeskompetenser tillsammans med Yrkesgrupper [#380](https://trello.com/c/Hq2V30el/380)
- Slutat skicka fel till Sentry när vi utvecklar lokalt [#895](https://trello.com/c/1ZxHNiZ0/895)
- Fix för checkboxar i RTL-språk [#885](https://trello.com/c/ElfpYxUV/884)

### Sökgränssnitt v4.0.2 (I test 2017-11-10, Produktionssatt 2017-11-10)
- Profilsidan visar nu fler än en av varje under yrken, kompetenser, språk och yrkesönskemål [#1014](https://trello.com/c/brLol9ns/1014) (ett tag visades bara 1 yrke även om man hade 5 t.ex.)
- Arbetsgivare ser inte `Sök enskild person`, men istället boxen `Immigrationsstatus` där de kan söka på `AT-UND`, `Har samordningsnummer` och `Asylstatus`. Handläggare kan fortfarande söka som innan. [#1016](https://trello.com/c/3Jl8kocV/1016)

### Sökgränssnitt v4.0.1 (I test 2017-11-09, Produktionssatt 2017-11-10)
- Flyttat kommun till en egen box `Geografiskt område` på plats 4.
- Inmatning för `Samordningsnummer`, `Födelsedatum` och `Fritext` har fått en plus-knapp.

### Sökgränssnitt v4.0.0 (I test 2017-10-26, Produktionssatt ca 2017-11-03)
- Hanterar den nya taxonomin, med Yrkeskompetenser tillsammans med Yrkesgrupper [#380](https://trello.com/c/Hq2V30el/380)

### API v4.8.1 (I test 2017-10-19, Produktionssatt 2017-10-19)
- Representera kvinna/man korrekt i sökresultat. (https://trello.com/c/Wi5P0KiF/885-frontend-s%C3%B6k-uppfylla-kraven-man-kvinna-del-av-567)
- Förhindra att autentiserade användare utan roll får någon som helst behörighet i jobskills.se.(https://trello.com/c/PWcGqRVf/889-roller-f%C3%B6r-olika-beh%C3%B6righeter-%C3%A5tkomst-till-s%C3%B6k)
- Representera samordningsnr korrekt i PDF export (https://trello.com/c/9Asln4C3/886-pdf-och-mail-samordningsnummer-ja-blir-nej-del-av-595)
- Strikt sökning fungerar nu korrekt för taxonomi-filter (https://trello.com/c/7kV168RF/843-mailutskick-%C3%B6ppen-s%C3%B6kning-eller-exakt-s%C3%B6kning-del-av-484)

### API v4.8.0 (I Test 2017-10-12, Produktionssatt 2017-10-19)
- Möjliggör visning av uppfyllt/ej uppfyllt på personuppgifter, t.ex. kön, ort, migrationsstatus [#567](https://trello.com/c/RwMpT2h2/567)
- Sparar om använaden har utbildningsdokument, samt engelska utbildningsdokument [#543](https://trello.com/c/9Hk4sosU/543)
- Sparar om användare väljer att inte vill ha massutskick [#659](https://trello.com/c/Rpl0HbxS/659)
- Sökanvändare kan välja att söka på alla som har eller inte har samordningsnummer [#857](https://trello.com/c/JAv3RBjq/857)

### Inmatningsgränssnitt v3.10.1 (I test 2017-10-19, Produktionssatt 2017-10-19)
- Ignorerar fel för Safaris incognito mode [#892](https://trello.com/c/tfK16Ic4/892-quota-has-been-exceeded)
- Fixar omvänd logik för checkboxen för email optout. [#891](https://trello.com/c/SnRFU85P/891-emailoptout-rutan-%C3%A4r-ikryssad-n%C3%A4r-den-ska-vara-urkryssad-och-vice-versa)

### Inmatningsgränssnitt v3.10.0 (I Test 2017-10-12, Produktionssatt 2017-10-19)
- Användare kan klicka i att de har samordningsnummer (utan att behöva fylla i själva numret) [#595](https://trello.com/c/B0bjKNok/595)
- Användare kan fylla i att man har utbildningsdokument samt engelska sådana [#543](https://trello.com/c/9Hk4sosU/543)
- Användare kan fylla i att man inte vill ha massutskick [#659](https://trello.com/c/Rpl0HbxS/659)
- Hjälptexter i profilöversikten har lagts till för att underlätta för användaren att förstå vad de ska fylla i och var [#465](https://trello.com/c/MR9dJO4F/465-465-hj%C3%A4lptexter-i-profil%C3%B6versikt-m)

### Sökgränssnitt v3.6.0 (I test 2017-10-19, Produktionssatt 2017-10-19)
- Toggle för öppen/strikt sökning [#843](https://trello.com/c/7kV168RF/843)

### Sökgränssnitt v3.5.0 (I Test 2017-10-12, Produktionssatt 2017-10-19)
- Man kan söka på kandidater som har utbildningsdokument samt engelska utbildningsdokument [#543](https://trello.com/c/9Hk4sosU/543)
- Man kan begränsa sin sökning till alla användare som har eller inte har samordningsnummer [#857](https://trello.com/c/JAv3RBjq/857)  

### API v4.7.1 (I Test 2017-09-27, Produktionssatt 2017-09-28)
- För att få till checkboxen för valet `Jag har ett samordningsnummer` har det möjliggjorts att spara `null`-värden på användare i API:et [#853](https://trello.com/c/V7tZz8tC/853)
### API v4.7.0 (I Test 2017-09-27, Produktionssatt 2017-09-28)
- Svensk body tillaggt på alla massutskick [#842](https://trello.com/c/ov4gt1YL/842)
- Ny kolumn skapad i databasen för `has_coordination_number` för att möjliggöra att man ska kunna klicka i checkboxen utan att behöva fylla i ett samordningsnummer [#848](https://trello.com/c/IXOvgEFH/848)
- User-queryn i GraphQL returnerar nu `email_opt_out` så att gränssnittet kan se om man vill få mailutskick eller ej [#851](https://trello.com/c/UavAVKQ2/851)
- Fix av behörigheter som möjliggör att skicka sitt CV per mail igen [#846](https://trello.com/c/gTLf08YJ/846)

### Sökgränssnitt v3.4.1 (I Test 2017-09-27, Produktionssatt 2017-09-28)
- Knappen `E-post-utskick` döljer inte längre antalet matchande kandidater i IE11 [#825](https://trello.com/c/dBPhDnkm/825)
- Fix av språk-flikarna [#827](https://trello.com/c/X9zrhBMH/827)
- Fix där paginerings-läknarna inte hamnar över sökresultat, samt att bara ett begränsat antal visas när det finns många sökresultat [#749](https://trello.com/c/GkE0y1uN/749)

### Inmatningsgränssnitt v3.9.3 (I Test 2017-09-28, Produktionssatt 2017-09-28)
- Lagt tillbaka översta login-knappen på Start-sidan [#854](https://trello.com/c/hwEYRMSW/854)
- Tagit bort console error som klagar när det inte finns några nyheter

### Inmatningsgränssnitt v3.9.2 (I Test 2017-09-27, Produktionssatt 2017-09-28)
- `Återställ val`-knapparna tar upp en egen rad även på större mobiler [#844](https://trello.com/c/8t68MKQR/844)
- Valet `Jag har ett samordningsnummer` sparas [#595](https://trello.com/c/B0bjKNok/595)
- `Logga in`- och `Registrera`-knapparna är tillbaka i mitten på Start-sidan på RTL-språk [#831](https://trello.com/c/fzec4eq2/831)

### Inmatningsgränssnitt v3.9.1 (I Test 2017-09-27, Produktionssatt 2017-09-28)
- Fix av diverse IE11 buggar [#831](https://trello.com/c/fzec4eq2/831)
- Frågetecknet för samordningsnumret har flyttats [#644](https://trello.com/c/QdaBtORO/644)
- Sidan som visas när tjänsten inte kan nås visar texterna på rätt språk [#614](https://trello.com/c/n9o9UbxK/614)
- När man försöker mejla sitt CV stängs modalen oavsett om det lyckas eller ej (det hamnar därmed inte under modalen som innan) [#829](https://trello.com/c/RbplowLw/829)
- Fix av Publicera-knappen där det kunde se ut som att man var publicerad och opublicerad samtidigt [#847](https://trello.com/c/adj8W0ba/847) & [#839](https://trello.com/c/iuP8Zu46/839)
- Ändrat ordning så att `Sök från lista` är default istället för fritext `Sök` [#838](https://trello.com/c/MaQtdKVo/838)
- Nyhets-kolumnen döljs när det inte finns några [#821](https://trello.com/c/EJVrLlvu/821)
- Kompetenser läses in på nivå 3 [#380](https://trello.com/c/Hq2V30el/380)
- En massa styling-fixar [#808](https://trello.com/c/qdhL3y9L/808) & [#844](https://trello.com/c/8t68MKQR/844)

### Sökgränssnitt v3.4.0 (I Test 2017-09-22, Produktionssatt 2017-09-28)
#### Features och fixar:
- Man kan nu skicka mail från Jobskills Admin [#484](https://trello.com/c/io5SRdRj/484)
- Uppdaterad sortering av sökresultat [#556](https://trello.com/c/H9uO5sW4/556)
- Lathunden har uppdaterats till v2.0 [#799](https://trello.com/c/KIq4Rw2b/799)
- Navigation-bar [#640](https://trello.com/c/T3Q4at9u/640)

#### Följande större features och fixar har gjorts i samband med mailutskick:

  - HTML-editor för att skriva mailutskick [#748](https://trello.com/c/LW8uF4vX/748)
  - Kunna ta bort mailutkast [#754](https://trello.com/c/pTIBhf9B/754)
  - Utskick-sida med översikt av sina utkast och skickade mail [#744](https://trello.com/c/rhgnS4zp/744)
  - Kontroller har lagts till så att bara behöriga kan se och göra mailutskick [#806](https://trello.com/c/0KKpmxIy/806), [#747](https://trello.com/c/sagBMjcv/747)

#### Samt dessa som uppstått och fixats under utveckling, som rör mailutskick:

  - `Spara Utkast`-knappen stänger och öppnar modalen igen [#807](https://trello.com/c/JJInzXVV/807)
  - Länkinmatningen har fixerats längst ner i email-inmatningsfältet för att alltid vara åtkomstbar [#813](https://trello.com/c/zAN9P2MY/813)
  - Emal-inimatningsfältet laddar in rätt texter när man öppnar ett utkast [#769](https://trello.com/c/N1Y9LT3i/769)
  - Fixat bugg där det inte gick att öppna ett utkast igen efter att man stängt det [#771](https://trello.com/c/PebxlVsK/771)
  - Endast behöriga kan se knappen för att göra mailutskick [#760](https://trello.com/c/ftz6EkUB/760)
  - Skicka och Spara Utkast-knapparna är disabled (dvs går inte att klicka på) medan mail sparas/skickas [#815](https://trello.com/c/jXJeYE4Q/815), [#816](https://trello.com/c/ogU7CTlj/816)
  - Fixat bugg där språket laggade efter i Ämnesraden [#763](https://trello.com/c/uSucITsM/763)
  - Gjort utskick modalen scrollbar för att rymma allt på mindre skärmar [#780](https://trello.com/c/gXYne2Qd/780)
  - Skicka knappen disable:as när innehåll saknas på något av de krävda språken [#751](https://trello.com/c/YyGb8gUa/751)
  - Fix där utkast listan inte visades alls när man sökt på asylstatus, AT-UND [#777](https://trello.com/c/RTQ303Uo/777)
  - Gjort alla sökkriterier till blåa "taggar" på utskicks-sidan och i modalerna [#756](https://trello.com/c/DjI95DNG/756)
  - Ämnesraden och mail-innehållet töms på Alla språk när man stänger utkast-modalen på sök-sidan, för att förhindra att man inte råkar glömma kvar oönskat innehåll i något språk efter en ny sökning [#793](https://trello.com/c/mh8v166U/793) & [#817](https://trello.com/c/RRzIklre/817)
  - Fix av bugg där man tidigare matchade mot alla kandidater när man gått tillbaka till sök-sidan från utskick [#778](https://trello.com/c/YfExAtNq/778)
  - Det går att välja om man vill skicka på enskilda språk (matchade mot valda användares språk), eller om man ska defaulta till Svenska och Engelska [#758](https://trello.com/c/gNNw0T5r/758)
  - Hantering av RTL-språk i email-inmatningsfälten [#752](https://trello.com/c/R5eyeImw/752)
  - Fix där utskicks-sidan var helt tom efter att mail skickats [#759](https://trello.com/c/BKbfiG9L/759)
  - Borttagna utkast försvinner (nästan) direkt från utkast-listan [#775](https://trello.com/c/ZUd36L1g/775)
  - samt dessa [#802](https://trello.com/c/0mH7kKCI/802), [#800](https://trello.com/c/ME3Ehi1R/800), [#776](https://trello.com/c/dGMkT7uL/776), [#761](https://trello.com/c/BgedOFpZ/761), [#770](https://trello.com/c/qj4XZHYQ/770), [#764](https://trello.com/c/O2Rr9Zqx/764), [#784](https://trello.com/c/kRvmase4/784), [#814](https://trello.com/c/VZQSPZTC/814), [#755](https://trello.com/c/AxsYWCRI/755), [#753](https://trello.com/c/fXOGxqZ0/753)

### Inmatningsgränssnitt v3.9.0 (I Test 2017-09-22, Produktionssatt 2017-09-28)
- **Nyheter på startsidan** [#502](https://trello.com/c/iu8IaWNo/502)
- Fixat bugg där det inte gick att redigera i Arbetslivserfarenhet [#582](https://trello.com/c/pEAYoJNt/582)
- Ny design för checkboxar och radioknappar [#642](https://trello.com/c/GYi4aM0B/642)

Samt följande mindre fixar:
- Lagt till `Logga In`-knapp på Nyhets- och Nyhetsöversikts-sidorna [#805](https://trello.com/c/lnDo8DUm/805)
- Tagit bort felmeddelande vid för kort lösenord på Login-sidan [#700](https://trello.com/c/YYvwyLFc/700)
- Gjort om Kön till radiobuttons [#647](https://trello.com/c/6GKwjbRL/647)
- Uppdaterat copyn på `/unavailable`-sidan [#614](https://trello.com/c/n9o9UbxK/614)
- Ny look på Publicera-profil-knappen [#482](https://trello.com/c/otfbh7fk/482)
- Ta med "Text för nyanlända" från yrkesgrupper, yrkesbenämningar och kompetenser till Karriärguiden [#670](https://trello.com/c/ZKZADTHw/670)

### API v4.6.0 (I Test 2017-09-20, Produktionssatt 2017-09-28)
- Funktionalitet för att spara utskick [#655](https://trello.com/c/ja2TQsK4/655), skicka mail [#653](https://trello.com/c/LaG3PNql/653) , ta bort mailutkast [#694](https://trello.com/c/4ML4HPJJ/694), uppdatera utkast [#704](https://trello.com/c/h38PcOvA/704), ladda in alla utskick [#656](https://trello.com/c/jtW7u69t/656)
- Sökningar sparas (för att kunna användas senare när man ska göra mailutskick) [#674](https://trello.com/c/Ep5h5Y4P/674)
-Ändrat vilka personer som får vissa behörigheter [#803](https://trello.com/c/XLnJfcB4/803) & [#820](https://trello.com/c/YsCCPRp5/820)
- Tabeller och migrationer för att mappa mellan sökningar, utskick, användare m.m. [#654](https://trello.com/c/ucU2slxP/654) & [#686](https://trello.com/c/DhsBl07c/686)
- Lagt till autentisering för system-routes [#708](https://trello.com/c/jvQ7pWLr/708)
- Förbättrad sortering av sökresultat [#556](https://trello.com/c/H9uO5sW4/556)

### API v4.5.0 (I Test 2017-08-22, Produktionssatt 2017-09-28)
* Releasen fixar buggen med att användare skapade med Facebook saknar epost, eftersom numera hämtar vi den som är registrerad för användaren i Facebook. [#667](https://trello.com/c/bNM1YTEX/667)
* Vi skapar även admin-användare första gången admin-inloggningen används. Nästa gång inloggningen sker hämtas den tidigare skapade användaren. [#673](https://trello.com/c/mgekxALf/673)
* Detta är också ett första steg i att spara sökningar och email-utskick.

### API v4.4.0 (I Test 2017-08-09, Produktionssatt 2017-08-14)
* Stöd för sökning på flera kommuner. [#580](https://trello.com/c/692yUaTL/580)
* Omindexering av profiler tar bort avpublicerade profiler ur indexet. [#636](https://trello.com/c/2tvyHPaW/636)
* Sentry används för loggning av fel. [#606](https://trello.com/c/fmKJRGgJ/606)
* Förbättrad loggning av fel vid skickade av e-post. [#446](https://trello.com/c/8TefxoIt/446)
* Marknadsområden läggs in i databasen för användning för statistik. [#565](https://trello.com/c/dUd7E9aY/565)
* Bugfixar

### Sökgränssnitt v3.3.0 (I Test 2017-08-09, Produktionssatt 2017-08-14)
* Man kan nu söka på flera kommuner samtidigt [#580](https://trello.com/c/692yUaTL/580)
* Räknaren som visar antal sökresultat är tillbaka [#630](https://trello.com/c/7hkaadAD/630)
* Man kan nu söka på hela mailadresser i IE11 [#551](https://trello.com/c/yA6tfEgS/551)
* Fixat ordningen/positionering av introtext på Profilsidan [#557](https://trello.com/c/uGQ4s6ft/557)

### Inmatningsgränssnitt v3.8.1 (I Test 2017-08-14, Produktionssatt 2017-08-14)
* Tagit bort meddelandet på startsidan om att IE11 inte stöds

### Inmatningsgränssnitt v3.8.0 (I Test 2017-08-09, Produktionssatt 2017-08-14)
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
