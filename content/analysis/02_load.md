---
Title: Load
Description: About Load
---

Analys laddningstider
=======================

Uppgiften går ut på att utvärdera tre valfria hemsidor med fokus på laddningstid och eventuella förslag till förbättring med avseende användarens upplevelse vilket påverkas av sidans laddtid.

Urval
-----------------------

De tre hemsidorna jag har valt att utvärdera är, Avanza, Blocket och Dagens industri.  
Det är tre olika kategorier av sidor nömligen, bank, nyheter och annonsering, detta är ett medvetet val för att se om det är stora skillnader mellan olika kategorier.  
Kända och välbesökta hemsidor, inte minst av mig själv som besöker dessa sidor dagligen.
Se länkar till sidorna under referenser.

Metod
-----------------------

För min undersökning har jag använt Devtools i webbläsaren Chrome, PageSpeed Insight (https://pagespeed.web.dev/)
och Google Kalkylark för dokumentera mätresultat.  
För mätningarna med Devtools så laddades sidan tre gånger för att få fram medelvärde av mätningen, sidan laddas om med snabbkommandot, CTRL + Shift + R, för att sidan ska laddas om utan att använda cache.  
Vid anvädning av PageSpeed Insight, så skrivs URL:en in för sidan man vill analysera och man får fram resultat både för Mobile view och Desktop view.  
Mätningarna är sedan dokumenterade med hjälp av Google Kalkylark och infogade på rapportsidan.


Resultat
-----------------------

Dokumentera dina resultat från din studie. Berätta vad du kom fram till, vilka resultat du hittade och observerade.

<h3>Avanza:</h3>

![Screenshot Avanza](%assets_url%/img/avanza_prtsc.png){.pictme}

Avanza fick 36 i mobile prestanda och 79 i desktop prestanda av 100 som är max prestanda vid mätningarna med Google PageSpeed.  
Resultatet av Devtoolsmätningen i Chrome gav följande medelvärden,  
Antal resurser: 62,3  
Överfört i (mb): 0,904  
Total storlek (mb): 5,3  
DOM laddning (sekunder): 0,243  
Laddningstid (s): 0,868  

<h3>Blocket:</h3>

![Screenshot Blocket](%assets_url%/img/blocket_prtsc.png){.pictme}

Blocket fick 35 i mobile prestanda och 54 i desktop prestanda av 100 som är max prestanda vid mätningarna med Google PageSpeed.  
Resultatet av Devtoolsmätningen i Chrome gav följande medelvärden,  
Antal resurser: 137  
Överfört i (mb): 4,8  
Total storlek (mb): 9,4  
DOM laddning (sekunder): 1,35  
Laddningstid (s): 2,5  

<h3>Dagens industri:</h3>

![Screenshot Dagens industri](%assets_url%/img/di_prtsc.png){.pictme}

Dagens industri fick 19 i mobile prestanda och 51 i desktop prestanda av 100 som är max prestanda vid mätningarna med Google PageSpeed.  
Resultatet av Devtoolsmätningen i Chrome gav följande medelvärden,  
Antal resurser: 155  
Överfört i (mb): 2,4  
Total storlek (mb): 6,9  
DOM laddning (sekunder): 0,9  
Laddningstid (s): 2,22  

<h3>Rådata för mätningarna:</h3>
<iframe class="dataexcel" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRxc45do3ZCOjWcGDuOneXCGnQ-mMkAgArIhckrIYgJjptBGRnnWDQnbfrSQFGekuKJMdfhPvgT_kZ0/pubhtml?widget=true&amp;headers=false"></iframe>

Analys
-----------------------

Det som förvånade mig mest i denna undersökningen var hur dålig prestanda sidorna fick i Mobile view. Resultat under 50 är dåligt, 50-89 är okej och 90-100 är bra. Samtliga tre sidor hade under 50. Avanza 36, Blocket 35 och Dagens industri 19.  
Samtliga tre sidor hade över 50 i Desktop view, bäst hade Avanza med 79 sedan kom blocket med 54 och Dagens industri med 51.  

PageSpeed ger följande förslag till förbättringar på samtliga sidor, Reducera JavaScript som inte används. 
Andra exempel på förbättringar med väsentlig skillnad enlig PageSpeed:  
Minska påverkan från tredjepartskod är förslag för Dagens industri och Blocket.
Minska arbetsbelastningen på modertråden, samtliga sidor.  
Minska körningstiden för JavaScript, samtliga sidor.

Ett annat intressant förslag var att, Minska serverns första svarstid, endast ges som förslag på förbättring hos Dagens industri. Vilket jag tolkar som att Avanza och Blocket har bättre servrar.

Referenser
-----------------------

- https://pagespeed.web.dev/
- https://www.avanza.se/
- https://www.blocket.se/
- https://www.di.se/

Övrigt
-----------------------

Rapporten skriven av Daniel Bondesson. December 2023.