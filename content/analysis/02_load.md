---
Title: Laddningstid
Description: Page about loadingtime
Template: analysis
Icon: hourglass-half-regular
---

# ![Hourglass](%base_url%/assets/svg/hourglass-half-regular.svg){.icon}  Laddningstid

Syftet med denna rapport är att få en större förståelse för vad som påverkar en webbsidas laddningstid och -storlek och hur vi kan påverka den i vårt arbete då vi utvecklar webbplatser. 


<div class="svg-container">
  <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="40">
    <path
      d="M0,20 Q50,0 100,20 T200,20 T300,20"
      fill="none"
      stroke="#e7def1b0"
      stroke-width="3"
    />
  </svg>
</div>



## Urval

Jag valde tre webbplatser med väldigt olika syften. Det första jag gjorde var att göra ett återbesök till [SVT](https://svt.se) från den första rapporten/analysen. Detta beslut tog jag enbart för att jag var nyfiken på vad en så pass avskalad, men ändå informationsfylld, sida skulle kunna hamna på i mätningarna. 

Den andra sidan jag valde var [BTH](https://bth.se) - detta för att det kändes relevant att ha med något som har med lärosätet att göra.

Sist men inte minst, valde jag webshoppen [Lyko](https://lyko.com/sv). Jag misstänkte att den skulle vara ganska tung då det är mycket bilder, banners och interaktiva element på samtliga sidor till skillnad från de två tidigare.  

<div class="svg-container">
  <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="40">
    <path
      d="M0,20 Q50,0 100,20 T200,20 T300,20"
      fill="none"
      stroke="#e7def1b0"
      stroke-width="3"
    />
  </svg>
</div>


## Metod

För att få fram någon typ av resultat har jag använt Google *PageSpeed Insights* samt Chrome Dev tools. PageSpeed Insights används för att analysera hur en webbsida presterar på både mobila enheter men även datorer. Vi får en väldigt detaljerad rapport som först ger oss ett “Passed” eller “Failed” resultat på *Core Web Vitals Assessment* vilket handlar om [Largest Contentful Paint](https://web.dev/articles/lcp), [Interaction to Next Paint](https://web.dev/articles/inp), [Cumulative layout Shift](https://web.dev/articles/cls), [First Contentful Paint](https://web.dev/articles/fcp) samt [Time To First Byte](https://web.dev/articles/ttfb). 

Under detta får vi även en sektion de kallar “Diagnose Performance Issues” där Vi först får betyg, från 0-100 där 100 är så bra det kan bli, utifrån Performance, Accessibility, Best Practices samt SEO.
Här får vi även förslag på hur man kan förbättra sin sida för att få ett bättre resultat och därmed även ge användaren en bättre upplevelse.


I Chrome DevTools har jag under *Network*-tabben tittat på hur mycket data som webbläsare tar emot från servern,i form av nätverksförfrågningar/requests. Här har vi dels “Transferred” men även “Resources” att titta på. Jag valde att, för att få ett så korrekt resultat som möjligt, göra mina mätningar i Inkognito-läge för att undvika att något cachas och därmed kan påverka resultatet.



<div class="svg-container">
  <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="40">
    <path
      d="M0,20 Q50,0 100,20 T200,20 T300,20"
      fill="none"
      stroke="#e7def1b0"
      stroke-width="3"
    />
  </svg>
</div>



## Resultat


<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSeKboN0UD1pAqnvlVpSUl8JIyb8wsx2-BVJ1ugm5e8zvhe4caDRmRix40YV89x1cKNz64USkGpJpua/pubhtml?widget=true&amp;headers=false" class="sheet" title="Embedded google sheet"></iframe>


![Svt Snapshot](%base_url%/image/svt-snap.png)


**SVT:** Jag blev inte speciellt förvånad över PSI resultatet som visar att SVT har resultat på mellan 96 och 100 på SEO, Best practices samt Accessibility på samtliga sidor jag testade. Däremot blev jag lite förvånad över Performance som på både Desktop men framförallt Mobile var lägre än jag trodde.
De två största problemen på huvudsidan, https://svt.se, är för mobil “First Contentful Paint” samt “Largest Contentful Paint “- på desktop är största problemet en “excessive DOM size”.

Gemensamt för båda lägena är att PSI bland annat föreslår att “Reduce unused JavaScript”, “Reduce unused CSS”, att bilder saknar explicit höjd och bredd.

Sidor jag tittat på: [svt.se](https://svt.se), [Inrikes nyheter](https://www.svt.se/nyheter/inrikes/) & [Om oss](https://omoss.svt.se/).


<div class="svg-container">
  <svg xmlns="http://www.w3.org/2000/svg" width="70%" height="40">
    <path
      d="M0,20 Q50,0 100,20 T200,20 T300,20"
      fill="none"
      stroke="#e7def1b0"
      stroke-width="3"
    />
  </svg>
</div>


![BTH Snapshot](%base_url%/image/bth-snap.png)

**BTH:** Personligen så upplevde jag inte laddningstiden som lång och blev därmed förvånad över det dåliga resultatet PSI gav samtliga tre sidor på Performance och även resultatet från network-mätningarna. På sidan [som visar upp program och kurser](https://www.bth.se/utbildning/program-och-kurser/) var “Largest Contentful Paint” uppe i så mycket som 13,130 ms, “Minimize main-thread work” landade på 4,5 sekunder och förslag om att “Reduce JavaScript execution time” låg på 2,9 sekunder. 

Kanske skulle man kunna se över vad som faktiskt måste laddas direkt och vad som kan elimineras eller åtminstone optimera i vilken ordning olika resurser och script laddas?

Sidor jag tittat på: [Bth.se](https://bth.se), [Program och kurser](https://www.bth.se/utbildning/program-och-kurser/) & [Det här är BTH](https://www.bth.se/om-oss/det-har-ar-bth/).


<div class="svg-container">
  <svg xmlns="http://www.w3.org/2000/svg" width="70%" height="40">
    <path
      d="M0,20 Q50,0 100,20 T200,20 T300,20"
      fill="none"
      stroke="#e7def1b0"
      stroke-width="3"
    />
  </svg>
</div>

 
 ![Lyko Snapshot](%base_url%/image/lyko-snap.png)


**LYKO:** Att en webshop som denna fick dåligt betyg i samtliga kategorier, inte grönt på en enda av de sidor jag valde att titta på, av PSI var både förvånande men samtidigt inte. Det är mycket bilder som laddas med både produkter, text och banners som ska locka till köp. 

Om vi enbart tittar på Accessibility-kategorin så ser vi att bildelement saknar alt-attribut, länkar saknar tillräckligt beskrivande namn, knappar saknar “accessible name”, kontraster är inte tillräckliga.. det är en ganska lång lista över saker som bör vara relativt lätta att justera och därmed underlätta besöket för samtliga användare.
“Larget Contentful paint element” tar 9,750 ms och även här hamnar “Minimize main-thread work” på 2,7 sekunder. Liksom både SVT samt BTH föreslås det att “Reduce unused JavaScript” och CSS.

Sidor jag tittat på: [lyko.com/sv](https://lyko.com/sv),  [Nyheter](https://lyko.com/sv/nyheter/products) & [Om Lyko](https://lyko.com/sv/om-lyko).




<div class="svg-container">
  <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="40">
    <path
      d="M0,20 Q50,0 100,20 T200,20 T300,20"
      fill="none"
      stroke="#e7def1b0"
      stroke-width="3"
    />
  </svg>
</div>


## Analys


Något som återkommit på samtliga sidor jag analyserat är att diagnosverktyget föreslår att korrigera “Largest Contentful Paint element”, “Reduce unused JavaScript", “Reduce unused CSS”, “Eliminate render-blocking resources”, att bilder ej har explicit satt höjd eller bredd och inte är “properly sized”. Att inte bara det jag själv skapar återkommande får dessa förslag känns lika delar betryggande som oroande. Att samma “problem” återkommer tyder på att det är något som kräver en del av utvecklare och inte alltid är det lättaste att lösa direkt - inte heller är det omöjligt att detta problem uppstår och blir än mer påtagligt desto större projektet växer sig.

Genomgående är att resultaten som uppmäts är bättre på desktop än mobile - vilket kanske inte är så oväntat då alla webbplatser och dess testade sidor får förslaget att “eliminate render-blocking resources” dvs se över hur script och stilmallar laddas/är optimerade.


Personligen anser jag att en sida som är tillgänglig för faktisk interaktion inom 4 sekunder är tillräckligt snabb, och inom den gränsen ligger alla dessa tre webplatser. Jag skulle nog säga att det, för mig, är mer irriterande med en sida som initialt verkar laddas snabbt - men där det plötsligt dyker upp till exempel en stor hero-banner/bild vilket rubber flödet, en cookiebanner eller reklam i bild eller videoformat och stör den interaktion man påbörjat.  


Om jag ska utse en vinnare i detta test är det solklart SVT som vinner. De hade nästan bara gröna resultat i PSI analysen och genomsnittsstorlek/laddningstid var även de lägsta. Det är inte så förvånande med tanke på motståndet Hade en webshop vunnit över en statlig nyhetskanal vars syfte är (eller åtminstone bör vara) att vara tillgängligt för alla och servera oss det viktigaste just nu - det om något hade varit en skräll.





<div class="svg-container">
  <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="40">
    <path
      d="M0,20 Q50,0 100,20 T200,20 T300,20"
      fill="none"
      stroke="#e7def1b0"
      stroke-width="3"
    />
  </svg>
</div>


## Referenser

Tilldelat utbildningsmaterial samt föreläsningar.

## Övrigt

Skrivet av Petra Johansson

