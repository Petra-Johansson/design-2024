---
Title: Färger
Description: About Colors
Template: analysis
Icon: fas fa-palette
---

# ![Palette](%base_url%/assets/svg/palette-solid.svg){.icon}  Färger


Syftet med denna uppgift är att analysera hur användandet av främst färger, men även typografi, kan påverka intrycket en webbsida ger. Speglar intrycket som ges av detta vad jag tror att respektive sidas syfte och mål är? 

## Urval

Jag valde att titta på tre webbplatser inom olika områden: [Csn.se](https://csn.se){.link}, [Svt.se](https://svt.se){.link} samt [ikea.se](https://ikea.se){.link}. 
Jag valde dessa tre då det är sidor som de flesta av oss troligtvis besökt åtminstone en gång och kanske att de till och med har en design som många direkt känner igen och/eller kan plocka fram ur minnet om man nämner namnen.


_________________

## Metod

För att begränsa något till vilka färger som skulle extraheras valde jag att enbart analysera det som hamnar “above the fold”.
Jag valde att använda mig av ["Adobe Color"](https://color.adobe.com){.link} och då specifikt funktionen ["Extract theme"](https://color.adobe.com/create/image){.link} för att först använda en snapshot av respektive webbplats och låta verktyget plocka ut de färger som sidan består av. 
Ett “problem” som uppstod i denna process var att verktyget gärna valde att plocka ut (utmärkande) färger från bilder som inte har något med själva sidan och dess färgschema att göra. Det var dock lätt korrigerat genom att flytta på markörer till bättre passande platser. 

Jag gick sedan över till fliken ["Color Wheel"](https://color.adobe.com/create/color-wheel){.link} för att se hur färgerna ligger placerade gentemot varandra i färghjulet för att se om jag genom detta kunde utläsa vilken typ av färgschema det är (mest) likt. 

För att plocka ut vilka fonter sidorna använt sig av tittade jag enbart i webbläsaren på *Inspect -> Elements* och letade där upp font-family.  

_________________


## Resultat

### Ikea.se


Jag skulle tro att Ikea vill förmedla dels något lättillgängligt och stabilt (vilket kan finnas i blåa nyanser) men även lekfullt och energiskt (vilket är lätt förknippat med både gult och orange), och det tycker jag att deras val av färger och typsnitt gör.


#### Färgval

Ikea använder sig av ett *triadiskt* färgschema där de blåa, gula och orange/röda nyanserna ligger fördelade över färghjulet som bilden nedan visar. Som komplement har de även neutrala nyanser i nästintill svart respektive vitt.

<div class="company-snaps">
<img src="%base_url%/image/ikea.png" alt="Ikea snap" class="snapshot" width="350" height="150">
<img src="%base_url%/image/ikea-wheel.png" alt="Ikea color wheel" class="snapshot" width="150" height="150">
</div>

<div class="palette-div">
<table class="palette-table ikea-palette">
<tr>
<th>#0367A6</th>
<th>#F2C53D</th>
<th>#D9420B</th>
<th>#F2F2F2</th>
<th>#0D0D0D</th>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</table>
</div>


#### Typografi

Föga förvånande så har de ett eget typsnitt, vilket används över hela sidan: *"Noto IKEA"*.
Som fallback-fonter har de valt ut ett antal som är väldigt lika, samtliga är av typen *sans-serif*.


| Använding     | Font family |
| --------------| ----------- |
| H1-H3:        | Noto IKEA   |
| Brödtext:     | Noto IKEA   |
| Fallbacks:    | “Noto sans”, Roboto, “Open Sans”, system-ui, sans-serif |


_________________


### CSN.se

Jag skulle inte bli förvånad om CSN har en ambition om att framstå som pålitliga och tillgängliga för alla - samtidigt som man vill kännas lite "unga" och moderna. Om tanken är att *statlig myndighet &#8800; stelt och tråkigt* tycker jag att de absolut har lyckats. 

#### Färgval

CSN använder ett *analogt* färgschema där de lila, korallrosa samt gula färgerna ligger jämnt fördelade över färghjulet, vilket kan ses på bilden nedan.

<div class="company-snaps">

<img src="%base_url%/image/csn.png" alt="Csn snap" class="snapshot" width="350" height="150">
<img src="%base_url%/image/csn-wheel.png" alt="Csn color wheel" class="snapshot" width="150" height="150">
</div>


<div class="palette-div">
<table class="palette-table csn-palette">
<tr>
<th>#F2808A</th>
<th>#361D59</th>
<th>#482973</th>
<th>#F2C063</th>
<th>#F2F2F2</th>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td> </td>
<td></td>
</tr>
</table>
</div>


#### Typografi 

Csn använder fonten *"Source sans pro"* genomgående på sin sida. Naturligtvis har de även ett gäng fallback-fonter, samtliga av typen *sans-serif*.

| Använding     | Font family     |
| --------------| ----------------|
| H1-H3:        | Source Sans pro |
| Brödtext:     | Source Sans pro |
| Fallbacks:    |  system, -apple-system, "san francisco", roboto, "segoe ui", "helvetica neue", arial, sans-serif |



_________________



### Svt.se

SVT har troligtvis en tanke de vill tas seriöst, vara okomplicerade och lättillgängliga för alla - och det tycker jag abasolut att de lyckas med
både när det gäller typsnitt men även färger.
#### Färgval 

Svt har ett *monokromatiskt* färgschema vilket utgår från en röd färg och även inkluderar framförallt två ljusare bakgrundsfärger samt en mörkare textfärger.  


<div class="company-snaps">
<img src="%base_url%/image/svt.png" alt="Svt snap" class="snapshot" width="250" height="150">
<img src="%base_url%/image/svt-wheel.png" alt="Svt color wheel" class="snapshot" width="150" height="150">
</div>

<div class="palette-div">
<table class="palette-table svt-palette">
<tr>
<th>#D9204F</th>
<th>#FFFFFF</th>
<th>#E02E3D</th>
<th>#1B1B1B</th>
<th>#F2F2F2</th>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</table>
</div>

#### Typografi: 

SVT har precis som de två tidigare, valt att använda en och samma fontfamilj över hela sidan: *"Publik"*.
Som föregående har även Svt valt ett antal *sans-serif* fonter som fallback.

| Använding     | Font family     |
| --------------| ----------------|
| H1-H3:        | Publik          |
| Brödtext:     | Publik          |
| Fallbacks:    |  Helvetica, Arial, Nimbus Sans L, Bitstream Vera Sans, sans-serif |


_________________



## Analys

Samtliga sidor har några färger som känns väldigt primära, men om man tittar i *Inspektera -> Elements* och går igenom alla färger som finns definierade ser man att det är enormt många. Många som jag inte ens lyckades se då jag klickade mig runt.
Precis som att sidorna har många olika färger definierade (ofta i :root ) har de även många fonts. Inte helt oväntat använde samtliga sidor sig av *sans-serif* fonts vilka är lätta att läsa på skärm. 

Samtliga sidor nyttjar även mycket whitespace och har även ljusa bakgrundsfärger, vilket är väldigt skönt i och med att de andra färgerna de har alla tar ganska mycket fokus. Det ljusa, men inte helt vita, bidrar till en balans och rymd.  


När det kommer till respektive sida skulle jag vilja påstå att **Ikea**’s hemsida utstrålar dels något tryggt med den lugna, blåa nyansen, men även energi och lekfullhet med de orangea och gula nyanserna. I och med att detta är tre relativt starka färger passar det fint med den gråvita bakgrunden och nästintill svarta textfärgen.


 Det är kanske inte jätteförvånande att **CSN** använder två olika lila nyanser på sin sida då lila ofta förknippas med både kunskap, kreativitet och lyx *(och visst är det väl ändå lite lyxigt att vi nästan får betalt för att utbilda oss?)*.
 Den korallrosa nyansen som främst används i header-bannern, drar till sig ens fokus utan att vara aggressiv samtidigt som den gula, vilken främst används på cta-knappar, ofta förknippas med optimism och glädje.


 **SVT** har en sida vilken känns väldigt okomplicerad, lättillgänglig och seriös med sina färg och typsnittsval. Om man jämför med andra nyhetssidor som till exempel [Aftonbladet](https://aftonbladet.se){.link} eller [Expressen](https://expressen.se){.link}, utstrålar Svt's en större seriositet och ett lugn de andra saknar.

_________________

## Referenser

Det enda jag egentligen nyttjat utöver läromaterialet är att läsa lite om färgers betydelse på bland annat [Arkitekt Kopia](https://www.arkitektkopia.se/akademi/vad-betyder-fargerna/){.link} och [Limetta webbyrå](https://limetta.se/tips-metoder-for-digitala-projekt/Fargpsykologi-Fargers-betydelse-och-effekt-pa-webben/){.link} då jag valde att inte ansluta mig till någon grupp för att disskutera med andra i kursen.


## Övrigt

Skrivet av Petra Johansson
