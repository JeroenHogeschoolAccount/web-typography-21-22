# Web Typography, 2020/2021

Als je doof bent, of als je om een andere reden geen geluid kunt horen, dan mis je veel informatie als je een film kijkt. Knisperende voetstappen, langzaam aanzwellende muziek, nerveus getik op een deur, je hoort het natuurlijk allemaal niet. Nu bestaat er zoiets als *closed caption*, wat een type ondertiteling is waarbij ook dingen als omgevingsgeluiden en de muziek beschreven worden. Hierdoor krijgt een kijker die informatie wel binnen.

Alleen wordt die auditieve informatie nogal neutraal beschreven. Het geluid van huilend persoon zou bijvoorbeeld beschreven kunnen worden als *snikgeluid op de achtergrond*. En iemand die lacht zou geschreven kunnen worden als *iemand lacht.* Heel neutraal, bijna zakelijk, en bovendien allebei in precies hetzelfde neutrale lettertype. Terwijl het toch echt over twee heel verschillende emoties gaat. 

Dat kan visueel sterker. 

En dat gaan jullie doen.

## Leerdoelen

- Je kan de kennis over vormgeving die je hebt opgedaan tijdens de minor technisch toepassen met behulp van CSS
- Je kan verborgen nuance uit een audiotrack overtuigend vertalen naar visuele (typografische) beelden
- Je kan je typografische keuzes onderbouwen.
- Je hebt de exclusive design principles gebruikt.

## Oplevering

Je levert een werkende versie op, gemaakt met HTML, CSS en JavaScript. Deze staat op Github. In een duidelijke readme documenteer en onderbouw je je ontwerpkeuzes. Je developmentgeschiedenis is terug te vinden op GitHub.

Je levert ook een *screen recording* met audio op van je fragment. Dit is een video van de definitieve versie, gemaakt van jouw browserscherm.

De beoordeling is mondeling en volgt [de rubric uit het beoordelingsformulier](web-typografie-beoordeling.pdf).

## Typografische restricties

Je *moet* een van deze twee opties kiezen, en je keuze moet je onderbouwen. In je readme staat een uitleg over je overwegingen om de ene of de andere restrictie te kiezen.

### Optie 1: Systeemfont

De eerste optie is dat je gebruik maakt van het zogenaamde *systeemfont* van degene die naar jouw werk kijkt. Dit font verschilt per operating system, en het verschilt soms zelfs per versie van het operating system. Het is ook aan te passen door de gebruiker zelf. 

Je hebt dus geen controle over welk lettertype er precies gebruikt wordt. Het levert dus een onzeker, en beperkt typografisch palet op. Je hebt geen *light* versies, of *extrabold*. En ook geen serif en sans-serif versie van dezelfde familie. In dit geval heb je alleen de beschikking over normal, **bold** en _italic_. Dit heeft natuurlijk ook zijn voordelen!

### Optie 2: Brenner

Je kan er ook voor kiezen om gebruik te maken van de complete Brenner familie. Dit is een zeer uitgebreid en uiterst flexibel font. [Hier kan je je verdiepen in dit font](https://www.typotheque.com/blog/brenner_an_unusual_typeface_family_with_distinct_voices). Als je kiest voor dit font dan heb je de beschikking over een *sans serif*, een *condensed*, een *serif*, een *monotype*, een *slab*, een *display* en een *script* versie. En veel van deze versies hebben varianten van *light* tot *bold*, en allemaal zowel *bold* als *italic*.

Met Brenner zijn er natuurlijk veel en veel meer mogelijkheden dan met systeemfonts. Dat kan zowel een voordeel als een nadeel zijn. 

Voor een overzicht, zie [de brenner.pdf](brenner.pdf).

## Het fragment

Ik heb een fragment voorbereid. Het gaat om twee scenes uit *Blade Runner 2049*. De captions staan in de HTML, en ze verschijnen in sync met de video. [Kijk maar](closed-captions/index.html).

### De captions

De captions staan in de html, in het bestand index.html. Je kan aan elke paragraaf eventueel een of meer classes toevoegen. Bijvoorbeeld `voice1` of `voice2 soft`. Classes voeg je handmatig toe in de html.

Met JavaScript worden er een paar dingen extra gedaan: 

- er wordt aan elke paragraaf een unieke class toegevoegd (`p0`, `p1`, etc)
- Elk woord wordt in een aparte `span` gezet. Hierdoor kan je elk woord apart stylen, en eventueel ook [na elkaar laten verschijnen](https://github.com/cmda-minor-vid/web-typography-18-19/blob/master/closed-captions/css.css#L41).

### Tijdens het afspelen

Tijdens het afspeelen wordt er een class `on` op de caption gezet als hij moet verschijnen, en een class `off` als hij klaar is. *Zowel class `on` als class `off` blijft op de caption staan!*

De timimg van de captions kan je aanpassen in [closed-captions/captions.js](closed-captions/captions.js).

Er verschijnen ook classes op de body op momenten dat er geluiden worden afgespeeld, zoals `sound1` en `sound2`. Je kan geluiden toevoegen in [closed-captions/sounds.js](closed-captions/sounds.js).

*let op,* de geluiden zijn niet compleet, dit zal je zelf moeten aanvullen.

## Een eigen fragment (afgeraden, uitgebreide onderbouwing is nodig)

Je kan er ook voor kiezen om een eigen, *beter* fragment te gebruiken. Dit wordt afgeraden. De tijd die je besteedt aan het zoeken naar dat fragment kan je beter besteden aan het werken aan de opdracht. Bovendien blijkt dat er vaak fragmenten worden gekozen die niet goed voldoen aan de opdracht. Als je een ander fragment kiest dan *moet* je dit goed onderbouwd voorleggen aan je docent. De deadline hiervoor is vrijdagochtend in de eerste week.

### Waar moet je op letten bij het kiezen van een eigen fragment.
Lees de opdracht nog eens goed door. Waar gaat het ook al weer precies om? 

Voor een goede onderbouwing van je keuze voor een ander fragment moet je deze vragen in elk geval beantwoorden:

- Welke informatie zit er in de audio die echt niet zichtbaar is?
- Welke rol speelt de audio in het fragment?
- Werkt de scene nog zonder geluid?
- Waarom is dit fragment beter dan het aangeboden fragment?

Je kan dan de nodige HTML en JavaScript genereren door gebruik te maken van [caption generator](https://cmda-minor-vid.github.io/web-typography-18-19/generator/) (in Google Chrome). 

Als je de closed captions wil bewerken dan kan je een tool zoals [Amber Script](https://www.amberscript.com/en) gebruiken. Daar kan je exporteren als `.srt`, en die kan je weer door de generator halen.


## Een eigen fragment (afgeraden, uitgebreide onderbouwing is nodig)

Je kan er ook voor kiezen om een eigen, *beter* fragment te gebruiken. Dit wordt afgeraden. De tijd die je besteedt aan het zoeken naar dat fragment kan je beter besteden aan het werken aan de opdracht. Bovendien blijkt dat er vaak fragmenten worden gekozen die niet goed voldoen aan de opdracht. Als je een ander fragment kiest dan *moet* je dit goed onderbouwd voorleggen aan je docent. De deadline hiervoor is vrijdagochtend in de eerste week.


# Deel student  


# Webtypografie 2021/2022
In dit document zijn mijn gemaakte keuzes en proces te lezen voor het vak Webtypografie. 

## Gekozen font

Ik heb gekozen voor het lettertype Brenner, hier konden we voor dit vak gratis gebruik van maken. Dit font heeft erg veel verschillende stijlen. Binnen elke stijl kan ook gekozen worden uit bold, light etc. Hierdoor leek het mij een goed idee om hiermee verder te gaan, in plaats van de tweede optie waar we voor konden kiezen: systeemfont.
Toen ik het overzicht van Brenner bekeek, had ik direct in mijn hoofd welke stijlen ik voor de stemmen kon gebruiken.  
Ik heb uiteindelijk gebruik gemaakt van drie verschillende stijlen.  Elke stem dat te horen is in de video heeft een andere Brenner stijl. Ik zal later onderbouwen waarom ik voor een bepaalde stem specifiek die ene stijl heb gekozen. 


## Het proces (updates) + onderbouwing

### Update 1 - 10 mei
Ik heb het fragment meerdere keren bekeken en beluisterd. Ik had nog niet eerder gehoord van de film Blade Runner 2049, dus ik kende het fragment nog niet. Ik heb eerst goed zitten luisteren naar de verschillende stemmen, zodat ik gemakkelijk voor elke stem kon bepalen welke Brenner stijl ik ga gebruiken. Ik heb drie verschillende stemmen waargenomen, echter vond ik het best lastig om voice1 en voice2 uit elkaar te houden. Voor voice1 heb ik gebruik gemaakt van "Brenner Mono". Dit lettertype lijkt op het lettertype dat vaak wordt gebruikt door machines/systemen. Ik vond dit lettertype daarom goed bij voice1 passen, aangezien deze stem niet bepaald menselijk klinkt (emotieloos). 
Voor voice2 heb ik gekozen om "Brenner Sans" te gebruiken. Dit lettertype is vrij neutraal, net zoals de stem. 
Voor voice3 heb ik gebruik gemaakt van vetgedrukt "Brenner Sans Condensed". Ik vond deze passen bij de random boze man. Dit font is breder en zwaarder, passend bij de boodschap van de tekst. 
Verder heb ik de video responsive in het midden gezet en groter gemaakt.
Ook heb ik door middel van het gebruik maken in CSS van "before" een korte vermelding toegevoegd wat wie welke tekst is, zodat dit voor dove mensen duidelijk wordt. Ik vond het zelf (met geluid) al lastig om stem 1 en stem 2 uit elkaar te halen, dus laat staan hoe lastig dit is voor mensen die doof zijn. Op dit moment heb ik dit beschreven met "Stem 1, stem 2 en stem 3", maar dit wil ik later nog veranderen. 
Als laatste heb ik de basis kleur van de body donker-grijs gemaakt, zodat dit beter past bij de video.


### Update 2 - 11 mei
Deze dag nagedacht welke effecten ik kan toevoegen. Ik ben begonnen met de eerste paar seconde van de video. Er is een zwaar en laag geluid te horen. Ik kreeg het idee om de video te laten trillen. Deze animatie heb ik met keyframes gemaakt in CSS. Verder wilde ik de twee felle kleuren (groen en roze) een extra 'laag' geven, door een box-shadow toe te voegen. Echter kreeg ik dit niet voor elkaar op de manier hoe ik het in gedachten had. 
Verder heb ik een effect gemaakt bij het geluid van het alarm, door de background van de body te laten knipperen met rode en blauwe kleuren. 


### Update 2 - 12 mei
Tijdens de les hulp gekregen van een medestudent met betrekking tot de box-schadow. Nadat ik de video via een andere manier in het midden had gezet (grid) was de box-schadow wel te zien. Deze heb ik vormgegeven. 
Op deze dag heb ik mijn tot nu toe gemaakte werk laten zien aan mijn ouders voor het krijgen van feedback, deze vroegen zich af of ik de tekst niet ook kon animeren. Dit wilde ik de volgende dag gaan doen.
Verder heb ik op deze dag te tekst verder vormgegeven, zoals kleur en stijl. Ik heb gekozen om voice1 de kleur lime te geven, omdat de stem mij moest denken aan een 'robot' stem. Programeertaal heeft ook vaak felle kleuren, zoals lime. Voice2 heb ik de kleur wit gegeven, omdat dit past bij de neutrale, rustige toon van de hoofdpersoon. Wit wordt geassocieerd met neutraal.  


### Update 3 13 mei
Deze dag ben ik aan de slag gegaan met de feedback dat ik van mijn ouders kreeg: het animeren van de tekst. Sommige belangrijke woorden heb ik geanimeerd, zoals wanneer de hoofdpersoon "Yes Sir" zegt. Deze woorden worden op het moment van uitspreken vergroot en veranderen van kleur. Ook heb ik de zin "interlinked within cells, interlinked within one stem." geanimeerd, door de letter-spacing langzaam te veranderen. Ik vond dit effect wel passen bij de zeer neutrale toon van de hoofdpersoon. Ik ga dit later nog testen of dit van toegevoegd belang is. Ook is er een animatie te zien bij de scheldende man. Deze tekst wordt rood en groot in beeld gebracht.  


### Update 4 14 mei
Ik heb zitten nadenken wat ik bij de scène waarbij de hoofdpersoon in een kleine kamer zit kan toevoegen. Ik vond dit best lastig, omdat er eigenlijk niet veel gebeurd. Er is wel een vervelende piep te horen. Ik heb daarom een vervelende trilling in de video en tekst toegevoegd. Ook veranderd de achtergrond langzaam naar rood (past bij spanning). 
Ik had wel soms moeite met het juist timen van de effecten. Dit heeft best veel tijd in beslag genomen, maar naar tientallen keren opnieuw proberen is het redelijk gelukt. Verder heb ik een beetje feedback verwerkt dat ik had gekregen. Het was bijvoorbeeld niet duidelijk dat de zin "Within cells interlinked." 3 keer werd gezegd (wanneer je geen geluid hebt). Dit heb ik opgelost door "after" te gebruiken. Achter de zin staat nu "3x". Ook heb ik op bij sommige woorden het contrast iets aangepast, zodat het beter is te lezen.  


### Update 5 15 mei
Wegens (medische) omstandigheden niet aan de opdracht kunnen werken.  


### Update 6 16 mei
Wegens (medische) omstandigheden niet veel aan de opdracht kunnen werken.  


### Update 7 17 mei
Deze dag ben ik begonnen aan het tweede deel van de video. Dit deel heeft een behoorlijk vreemd achtergrondgeluid. 





## Samengevat 

### Typografie
### Kleur
### Animatie

