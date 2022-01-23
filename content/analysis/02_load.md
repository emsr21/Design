---
Title: Loading times
Description: Loading times
Image: https://dbwebb.se/image/theme/leaf_256x256.png
ImageAlt: dbwebb löv
Template: analysis
---

Analys utav laddningstider
==========================

<img style="width: 100%" src="http://localhost:8080/dbwebb/design/me/portfolio/assets/img/robertSpaceIndustries.png" alt="Nature" class="responsive">

Jag har valt att analysera hemsidan [https://robertsspaceindustries.com/](robertsspaceindustries.com). Denna sidan är gjord av Cloud 
Imperium Games och den är designad för att sälja deras Star Citizen och Squadron 42. Anledningen till att jag valde denna sidan är för att 
jag är någorlunda insatt i vad dem gör som företag och jag gillar deras spel som jag har spelat ganska mycket.

<img style="width: 100%" src="http://localhost:8080/dbwebb/design/me/portfolio/assets/img/eneba.png" alt="Nature" class="responsive">

Den andra sidan jag valde är [https://www.eneba.com/sv/](eneba.com/sv) vilket är en sida som säljer spel nycklar till olika spelplattformar 
som Steam och Origin. Spelen som säljs är alltid billigare på sidan än om man köper dem från den riktiga launchern. Detta stämmer inte 
alltid om det skulle vara en stor rea på launchern man väljer att köpa till.

<img style="width: 100%" src="http://localhost:8080/dbwebb/design/me/portfolio/assets/img/eneba.png" alt="Nature" class="responsive">

Den tredje sidan jag valde var [https://www.ginza.se/](ginza.se), denna sidan säljer mediaprodukter, som film och musik. Den sidan valde 
jag för att jag brukar vara inne på den sidan ganska ofta och jag brukar köpa filmer på sidan. 

Jag gick in på sidorna och använde mig av devtools där jag använde mig av tabben network för att ladda om sidan utan cacheminne. Detta för 
att mäta laddningstiderna och för att kolla vilken fil som är störst och hur stor den är. Jag skapade ett google kalkylark där jag sparade 
all information från sidorna. Under min analys körde jag  tre sidor från varje webbplats i google Pagespeed för att få fram betyg och 
förslag på förbättringar. Jag har tagit snapshots på varje webbplats och lagt in på den här analyssidan. När min analys av de tre 
webbplatserna var klar så embedade jag arket på den här sidan.

De vanligaste förbättringsåtgärden för webbplatsen robertsspaceindustries.com är att skicka bilder i modernare filformat. På webbplatsen 
eneba.se finns två vanligaste förbättringsåtgärder och det är att reducera JS och att minska servens första svarstid. På Ginza.se är den 
vanligaste förbättringsåtgärden är samma som eneba.se men de borde ha ett modernare bildformat.

När jag rangordnar webbplatserna baserat på deras mätvärden så blir det så här:
1. Ginza
2. Eneba
3. RSI

Detta resultat kom fram genom att räkna ut medelvärdet de tre olika sidorna på PC och mobil. Medelsiffrorna är på Ginza 71 på PC och 28 på 
mobil. När det gäller Eneba blev resultatet 55 på PC och 20 på mobil. Den som rangordnas sist är RSI där värdet blev 24 på PC och 15 på 
mobil. Vinnaren i det här testet blev Ginza.

Webbpletserna har olika storlekar på sidorna då den största är RSI som har en storlek på 14,1 MB. De andra två är mycket mindre i 
jämförelse då eneba ligger på 6,3 MB och ginza på 3,4 MB.

Jag anser att en webbsida har en snabb laddningstid om den ligger mellan 2 - 4 sekunder. Tar den längre tid så är den långsam enligt mig. 
Alla webbplatserna i mitt urval startar snabbt enligt mig. Den snabbaste är Ginza.se med laddningstid på 2,35 sekunder på mitt nätverk. 
Siffran fick jag fram genom att beräkna medelvärdet mellan tre försök. De andra två ligger under 4 sekunder och strax över Ginzas tid.

Enligt mig kan webbplatsen Ginza förbättra sin sida på flera sätt. Ett förslag är att försöka optimera JS eftersom det är den största filen 
på hela sidan.

Webbplatsen Eneba kan förbättra sin sida genom att komprimera sina textfiler. De har all HTML kod på flera rader. De skulle istället kunna 
köra det i ett program som lägger all kod på en rad.

En förbättring som webbplatsen RSI kan göra är att göra samma sak som jag föreslog för eneba. De har däremot två stora .webm filer som har 
typ media och har en storlek på 3 MB sammanlagt då man förmodligen skulle kunna komprimera.

Emil Svedrin (emsr21)

<iframe style="width: 100%; margin-left: 0" src="https://docs.google.com/spreadsheets/d/e/
2PACX-1vQH0XTST8DqX7P_2F2AUNth-hv8NKoI_iINyG4_nHAIOBbUYZ3vDmkHUtkbVR2sKT0gywL9b9P-2jLG/pubhtml?widget=true&amp;headers=false"></iframe>
