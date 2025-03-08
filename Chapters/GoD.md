## GAME OF DRONES

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-01.jpg?height=1840&width=1620&top_left_y=719&top_left_x=187)
nlt module
voor vwo
versie 1.1

Deze nlt-module Game of Drones versie 1.1, is bestemd voor de lessen Natuur, Leven en Technologie (nlt). De module is op 19-12-2019 gecertificeerd door de
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-03.jpg?height=355&width=378&top_left_y=188&top_left_x=1567) Vereniging NLT voor gebruik in de domeinen:

| Vwo | E1: Methoden en technieken van technologische <br> ontwikkeling | E2: Processen en <br> producten |
| :--- | :--- | :--- |

De module is gecertificeerd tot 19-12-2024 met certificeringsnummer 6241-087-VE1E2.
De originele gecertificeerde module is in word- en pdf-formaat downloadbaar via: http://module-database.betavak-nlt.nl.

- De module is ontwikkeld door

Joshua Latukolan, Tim Noyce, Huib van Rijt, Leon Rozing, Alborz Salimian Rizi, Hector Santoni Gomez, Thomas Stolk en Godfried Wieske.

- Vakcoach en hoofdredacteur

Ir. Wim Sonneveld (SEC, TU Delft)

- Inhoudelijk expert

Ir. Dr. C.J.M. Verhoeven (Robotics Institute, EWI, TU Delft)
Aangepaste versies van deze module mogen alleen verspreid worden, indien in dit colofon vermeld wordt dat het een aangepaste versie betreft, onder vermelding van de naam van de auteur van de wijzigingen.

## Copyright © 2019 Vereniging NLT, Wijk bij duurstede

In 2024 is klein onderhoud aan de module uitgevoerd door Sander Haemers Bètasteunpunt TUDelft. De links zijn gecontroleerd en paragraaf 2.2 heeft een update ontvangen.

Deze module is ontwikkeld door leraren in opleiding als eindopdracht voor het vak Ontwerpen van Educatieve Producten en Processen (OvE) in de masteropleiding Science Education \& Communication van de TU Delft, onder verantwoordelijkheid van de Vereniging NLT. Deze heeft de copyrights overgedragen aan de Vereniging NLT.
De auteurs hebben bij de ontwikkeling van de module gebruik gemaakt van materiaal van derden en daarvoor toestemming verkregen. Bij het achterhalen en voldoen van de rechten op teksten, illustraties, enz. is de grootst mogelijke zorgvuldigheid betracht. Mochten er desondanks personen of instanties zijn die rechten menen te kunnen doen gelden op tekstgedeeltes, illustraties, enz. van een module, dan worden zij verzocht zich in verbinding te stellen met Vereniging NLT.
De module is met zorg samengesteld en getest. Vereniging NLT en auteurs aanvaarden geen enkele aansprakelijkheid voor onjuistheden en/of onvolledigheden in de module. Ook aanvaarden Vereniging NLT en auteurs geen enkele aansprakelijkheid voor enige schade, voortkomend uit (het gebruik van) deze module. Niets uit deze uitgave mag worden
verveelvoudigd, door middel van druk, fotokopieën, geautomatiseerde gegevensbestanden of op welke andere wijze ook zonder voorafgaande schriftelijke toestemming van Vereniging NLT.

## Inhoud

Colofon ..... 3
Voorwoord ..... 7
Opbouw van de module ..... 8
Lesschema ..... 8
0 Casus: Onderzoeksbasis in brand .....  9
Game of Drones ..... 10
R\&D opdrachten ..... 10
Vliegende Rechter ..... 11
Trivia ..... 11
Beoordeling ..... 11
1 Inleiding en Ontwerp ..... 13
1.1 Wat zijn drones? ..... 13
1.2 Onderdelen van een drone ..... 13
1.3 Ontwerpdossier ..... 14
1.4 Ontwerpcyclus ..... 15
2 Geschiedenis en maatschappij ..... 17
2.1 Geschiedenis van de drone ..... 17
2.2 Drones in onze maatschappij ..... 18
De Vliegende Rechter ..... 21
3 Besturingssysteem van drones ..... 22
3.1 Besturingssysteem ..... 22
3.2 ROS ..... 22
3.3 Hardware vereist voor het platform ..... 24
3.4 Softwarecomponenten ..... 24
3.5 Autopiloot en Drones ..... 26
De Vliegende Rechter ..... 29
4 Dataverzameling, snelheids- en plaatsbepaling ..... 30
4.1 Oriëntatie ..... 30
4.2 Snelheids- en plaatsbepaling ..... 30
De Vliegende Rechter ..... 33
5 Externe krachten op een drone ..... 34
5.1 De lift van een vleugel ..... 34
5.2 Luchtweerstand ..... 36
5.3 Vermogen ..... 37
5.4 Besturing ..... 38
De Vliegende Rechter ..... 41
Intermezzo ..... 42
6 Vervorming, interne krachten, materialen ..... 45
6.1 Vervorming ..... 45
6.2 Interne krachten ..... 47
6.3 Materialen ..... 48
De Vliegende Rechter ..... 51
7 Aandrijving ..... 52
7.1 Voortstuwing ..... 52
7.2 Energievoorziening ..... 54
De Vliegende Rechter ..... 57
8 Vliegende Rechter: Legal Clearance ..... 58
8.1 Wat is: ‘Legal Clearance'? ..... 58
8.2 Debat ..... 58
9 Final Game of Drones ..... 59
9.1 Game of Drones ..... 59
9.2 Ontwerpopdracht ..... 60
9.3 Strategie ..... 62
9.4 Presentatie ..... 62
9.5 (optioneel) Politieke problemen ..... 62
Bijlage Practicum ..... 64
Practicum 1 Spaghetti ..... 64
Practicum 2 Citroenkracht? ..... 65
Practicum 3 Waterkracht ..... 66
Bronnen ..... 67

Drones worden steeds gewoner. Begin deze eeuw werden ze alleen door het leger ingezet en hoorde je alleen iets over drones als er slachtoffers waren gevallen. Tegenwoordig kun je je eigen drone in de speelgoedwinkel kopen en kun je er bijna overal mee vliegen. Drones met verschillende functies worden door allerlei instanties en diensten ingezet in plaats van werkend personeel.

Maar waar bestaat een drone eigenlijk uit? Hoe blijft deze in de lucht en wat maakt een drone anders dan een bemand vliegtuig? Door te kijken naar het ontwerp van een drone voor een specifieke missie leer je niet alleen hoe alles werkt en wat de taak is van de verschillende onderdelen, maar ook waar de verschillen zitten en waarom je bij het ontwerpen bepaalde keuzes maakt. Waarom heeft een drone die een camera boven een wedstrijd houdt een rotor, maar heeft een drone die boven de woestijn naar terroristen zoekt vleugels? Waarom hebben we geen drones die op zonne-energie vliegen?

Tot slot kijk je naar de maatschappelijke impact. Drones zijn nog vrij nieuw en worden constant verbeterd. Men is nu pas bezig wetten regels en beperkingen op te stellen en die worden constant ingehaald door de techniek. Behalve de wettelijke issues zijn er ook ethische. Wat gebeurt er al iemand een drone ontwerpt die volledig autonoom kan opereren? Mag je die dan ook voor militaire doeleinden gebruiken? Wie is verantwoordelijk als een autonome drone tegen een gebouw aanvliegt?

Deze vragen ga je binnen een gestelde casus beantwoorden. Je gaat in groepjes een drone ontwerpen die (een deel van) de missie kan vervullen. Maar in de echte wereld is er nooit maar één bedrijf dat een ontwerp maakt en indient. Verschillende bedrijven concurreren om een opdracht binnen te halen. En hoewel je zou denken dat alleen de beste drone gekozen wordt, kun je nooit helemaal zeker zijn waarom een opdrachtgever een bepaalde keuze maakt. Je vormt met je groep een bedrijf, je krijgt een casus, je ontwerpt een drone en probeert deze te verkopen. De Game of Drones gaat beginnen...

## Opbouw van de module

Drones zijn gecompliceerde apparaten. Om toch een breed begrip mogelijk te maken zijn in deze module 9 hoofdstukken geschreven en een casus. De module is daarmee te groot om in zijn geheel te behandelen binnen de tijd die er op een gemiddelde school voor een nlt-module staat. Hierdoor zal niet elke leerling alle hoofdstukken kunnen bestuderen. Het is mogelijk om verschillende hoofdstukken door verschillende leerlingen parallel te laten bestuderen. Het is ook mogelijk om sommige paragrafen in zijn geheel over te slaan of delen ervan.

De casus, hoofdstuk 0 en hoofdstuk 2 zijn gericht op de maatschappij. De hoofdstukken 1 en 8 gaan deels over de maatschappij. In de hoofdstukken $3 \mathrm{t} / \mathrm{m} 7$ gaat het over de technische aspecten van drones. Het is aan de docent om te bepalen waar hij/zij de nadruk op wil leggen.

## Lesschema

Onderstaand een voorbeeld van een mogelijke lesplanner. In dit voorbeeld kiest de docent ervoor om de hoofdstukken 3 en 4 en ook de hoofdstukken 6 en 7 parallel door de leerlingen te laten bestuderen. De nadruk ligt op de eindopdracht waar veel tijd voor is ingepland.

Steeds aan het eind van een hoofdstuk geeft de R\&D-opdracht weer een stukje informatie en punten om de eindopdracht te kunnen maken.

| Contactuur | Route A | Route B |
| :---: | :---: | :---: |
| 1 | Casus |  |
| 2 |  |  |
| 3 | H1 |  |
| 4 |  |  |
| 5 | H2 |  |
| 6 |  |  |
| 7 | H3 | H4 |
| 8 |  |  |
| 9 | H5 |  |
| 10 |  |  |  |
| 11 |  |  |  |


| Contactuur | Route A | Route B |
| :---: | :---: | :---: |
| 12 | Intermezzo |  |
| 13 | H6 | H7 |
| 14 |  |  |
| 15 |  |  |
| 16 |  |  |
| 17 | H8 |  |
| 18 |  |  |  |
| 19 | H9 |  |
| 20 |  |  |  |
| 21 |  |  |  |

## 0 Casus: Onderzoeksbasis in brand

In het tropische regenwoud van Yeongyang-gun, Zuid-Korea, staat een onderzoeksbasis in brand. De basis staat op een voor de meeste voertuigen moeilijk bereikbare locatie. Dit is niet de eerste keer dat er een brand ontstaat en het zal ook niet de laatste keer zijn. De Zuid-Koreaanse regering wil een permanente methode hebben om met dit soort problemen om te gaan. Hoewel ze regelmatig voorkomen is de frequentie van dit soort branden erg laag. Daarom is het niet handig om bemande voertuigen te gebruiken, aangezien dit zou betekenen dat je permanent een bemanning op stand-by moet hebben die hoogstens een paar keer per jaar uitrukt. Het gemiddelde loon in Zuid-Korea is daarnaast ook erg hoog, dus is het verstandiger om voor onbemande voertuigen te kiezen. Hiervoor hoeft er geen complete bemanning permanent op stand-by te staan, de voertuigen kunnen lang opereren en er is geen kans op slachtoffers onder de reddingswerkers. De regering heeft een opdracht uitgeschreven, waaraan jij met je groep zult moeten voldoen.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-09.jpg?height=700&width=1756&top_left_y=1209&top_left_x=119)

Figuur 0.2 De onderzoeksbasis

De Zuid-Koreaanse overheid heeft gekeken naar de problemen die ze met drones willen oplossen en heeft vier kerntaken geformuleerd die ze moeten kunnen uitvoeren, namelijk:

- surveillance (frequentie!) en lokaliseren van het probleem;
- assisteren bij het redden van de mensen;
- assisteren bij het redden van de apparatuur;
- assisteren bij het blussen van de brand.

Het is mogelijk om een drone te ontwerpen die al deze vier taken kan volbrengen, maar dat is erg inefficiënt. Om deze reden heeft de ZuidKoreaanse overheid meerdere bedrijven aangeschreven, die allemaal een drone zullen ontwerpen die een deel van de taken kan uitvoeren. Een speciaal comité zal het uiteindelijke besluit nemen, welke drones gekocht zullen worden.

## Game of Drones

## GAMEOF

Je werkt in deze module in groepen van drie of vier leerlingen. ledere groep vormt een bedrijf. Zoals hierboven beschreven is, mag ieder bedrijf één drone ontwikkelen. Op welke taak je je wilt richten en hoe jouw drone die taak gaat uitvoeren, mag je helemaal zelf weten. Houd er hierbij wel rekening mee dat dit een opdracht is die aan een comité wordt voorgelegd. Het comité kiest niet per se voor de vier beste ontwerpen, maar kiest voor een combinatie die het beste de opdracht kan vervullen. Aan jullie is de taak om je net zo te gedragen als een bedrijf zou doen. Jullie hebben de mogelijkheid om een (informele) alliantie te vormen met een ander bedrijf. Bedenk hierbij dat niets onmogelijk is. Het heet niet voor niets Game of Drones.

- Je kunt ook nog andere criteria bedenken, waaraan jouw drone wel voldoet en die van de concurrentie niet.
- Een korte mediacampagne (presentatie) waarom jullie idee zo belangrijk is, kan jou naar de top brengen en al je concurrenten torpederen.
- De docent fungeert als het comité, eventueel in combinatie met anderen, daarbij heeft de overheid de autoriteit om allianties te weigeren. Bijvoorbeeld bij prijsafspraken, want die zijn verboden.
- De overheid kan de regels aanpassen, als er tussentijds verkiezingen zijn.
- Je kunt zelf formuleren wat naar jullie idee de klant echt zou moeten willen. Hierin kun je je onderscheiden van anderen.


## R\&D opdrachten

Het doel van deze module is om zoveel mogelijk informatie aan te reiken, zodat jullie bedrijf een weloverwogen keuze kan maken voor het type drone die jullie willen ontwerpen. Daarnaast heeft elk hoofdstuk een of meer Research \& Development (R\&D) opdrachten. Daarmee kun je 'Budget' verdienen om je drone te bouwen. Per hoofdstuk kun je voor een onderdeel van de drone zogeheten R\&Dpunten verdienen. Aan het einde van de module heeft het ene team meer keuzes dan het andere team, want met meer punten kan je meer uitgeven aan onderdelen.
Je kunt dan bijvoorbeeld meer technische onderdelen kiezen om de drone te bouwen of onderdelen die betere prestaties kunnen leveren?

Het thema van het hoofdstuk waar de punten zijn verdiend, is dan ook waar je de punten aan kunt uitgeven.
Het ontwerp van de drone is verdeeld in 5 onderdelen:
Besturingssysteem (Hoofdstuk 3), sensor (Hoofdstuk 4), vleugels of rotor (Hoofdstuk 5), romp (Hoofdstuk 6) en aandrijving (Hoofdstuk 7).

Voor elk van die onderdelen maak je keuzes gebaseerd op de missie en de eisen aan je drone. De hoeveelheid keuzes die je beschikbaar hebt hangt af van je verzamelde R\&D-punten.

Voor elke R\&D-opdracht kun je punten halen die je voor een onderdeel kunt inzetten. Hoe meer R\&D-punten je hebt verzameld, hoe meer keuzes je hebt voor het ontwerp van je drone. Voor elke R\&D-opdracht geldt:

- Onvoldoende = 0 punten
- Voldoende $=1$ punt
- Goed $=2$ punten
- Uitzonderlijk = 3 punten
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-11.jpg?height=213&width=395&top_left_y=676&top_left_x=336)


## Vliegende Rechter

Het vak nlt is dan vooral een technisch of bèta gericht vak, maar jullie ontwerpen hebben wel invloed op de maatschappij om ons heen. Om deze reden is er de Vliegende Rechter. In een aantal hoofdstukken heb je hierbij verhalen en/of opdrachten. Deze opdrachten zijn niet technisch, maar wel belangrijk. Ze hebben te maken met wat drones doen met de maatschappij, en hoe de samenleving en de wet ermee omgaan. Zorg ervoor dat je de antwoorden van deze opdrachten zorgvuldig bijhoudt, want ze zijn belangrijk om voor jouw drone ‘legal clearance' te krijgen. Dat betekent dat je minimaal 70\% van de opdrachten van de Vliegende Rechter succesvol moet hebben afgerond voordat je toestemming krijgt om naar het laatste hoofdstuk te gaan, het ontwerpen van de drone.

## Trivia

Game of Drones heeft zijn titel geleend van de serie Game of Thrones. Wie de serie kent, weet dat we niet een vergelijkbare setting kunnen bouwen. Toch zul je merken dat er een aantal elementen van de serie terugkomt in dit project. In de serie volg je het verhaal van een aantal grote families die allen aanspraak maken op de felbegeerde troon in het fictieve land Westeros. Jullie bedrijf staat voor een van de families en de casus is de troon. Elementen uit Game of Thrones die je zult tegenkomen in Game of Drones: - je kunt allianties vormen;

- de wetten (=spelregels) kunnen aangepast worden tijdens het spel; - geld (=punten) speelt een belangrijke rol.


## Beoordeling

Het eindresultaat van de game is het ontwerp van een drone. Uit de ontwerpen kiest het comité de drones die gekocht worden om de missie uit te voeren. Dit is echter niet het enige wat je voor dit hoofdstuk in moet leveren. Je maakt een ontwerpdossier, waarin al je R\&D opdrachten verwerkt zijn. Dit dossier, in combinatie met je ontwerp en de presentatie geeft je cijfer voor deze module.

Je ontwerp bestaat uit je keuzes van de vijf onderdelen met daarbij een onderbouwing, waarom je voor deze onderdelen hebt gekozen en hoe dit bijdraagt aan het uitvoeren van de gekozen missie. Mooie schetsen, of simulaties worden natuurlijk ook gewaardeerd door de politici in het comité die de uiteindelijke keuze maken.

Alle ontwerpen worden uiteindelijk beoordeeld op 7 categorieën:
Aanschafkosten (dure of veel materialen kosten meer).

Operationele kosten (onderhoud, vervanging en brandstofverbruik).
Time in the air (Hoe lang kan de drone in de lucht blijven)

Wendbaarheid (kan de drone stil hangen? Hoe groot is de minimumsnelheid)
((ly))
Bereik

Veiligheid (hoe stevig is de drone, hoe robuust zijn de systemen)

Laadcapaciteit.

Je ziet dat vijf van de zeven categorieën betrekking hebben op functies van de drone. Alle ontwerp-onderdelen van de drone hebben in deze categorieën een waarde tussen -10 en 10. Waarbij 10 betekent dat een onderdeel heel goed is en -10 dat het heel slecht is. Bijvoorbeeld: grote vleugels zorgen voor veel lift bij een lage snelheid en zijn dus goed voor vliegtijd. Ze zijn redelijk goed voor de operationele kosten vanwege een lager brandstof verbruik. De lage snelheid is enigszins slecht voor het bereik van de drone en groter vleugels zijn ook niet goed voor de wendbaarheid. De aanschafkosten zijn ook hoog vanwege het gebruik van meer materiaal. De grotere vleugels bieden wel meer laadruimte. De score van grote brede vleugels zou dan kunnen zijn: A -2, O +2, T+6, W-2, B-2, V 0, L +4.

## R秉D

Opdracht: De eerste stap
Voor je als bedrijf je ontwerp kunt indienen, moet je een bedrijf vormen. Wat je hiervoor nodig hebt is een naam, een logo en een motto, zodat iedereen weet waar jouw bedrijf voor staat. De naam moet fijn in de mond liggen en is het eerste uithangbord voor je bedrijf. Je logo kan te maken hebben met wat dat je gaat ontwerpen, maar het kan ook iets sentimenteels zijn, of gewoon een mooi figuurtje. Je motto geeft in een paar woorden weer waar je als bedrijf voor staat. Let wel op dat er geen copyright rust op je logo of motto, dat zou namelijk een dure rechtszaak kunnen worden.

Hierna ga je een eerste idee vormen van wat voor drone je zou willen maken. Dit hoeft nog niet technisch onderbouwd te zijn, maar is een schets van hoe volgens jouw bedrijf een drone eruit zou moeten zien.

## Maak en lever in:

R\&D 0a Ontwerp een logo, naam en motto voor jullie bedrijf. R\&D Ob Maak een eerste schets van de ideale drone.

## Beloning:

Het comité neemt je ontwerp alleen in overweging, wanneer er een bedrijfsnaam, logo of motto op de cover staat.

## 1 Inleiding en Ontwerp

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-13.jpg?height=393&width=589&top_left_y=563&top_left_x=142)

Figuur 1.1 Tello Edu, Rob Lamping
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-13.jpg?height=458&width=598&top_left_y=1276&top_left_x=132)

Figuur 1.2 SeaFox AUV by Altas Elektronik
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-13.jpg?height=315&width=580&top_left_y=1981&top_left_x=144)

Figuur 1.3 Schematische tekening van een drone. Bron: DJI.nl

Drones zijn niet meer weg te denken uit onze maatschappij. In de krant en op televisie hebben ze het vaak over de nieuwste ontwikkelingen rondom drones. Maar wat zijn drones eigenlijk?

In dit hoofdstuk krijg je een korte introductie in Drones, en zul je daarnaast een eerste stap maken in het ontwerpen van een drone. Daarbij komen de volgende punten aan de orde:

- Wat zijn drones?
- Onderdelen van een drone
- Ontwerpdossier
- Ontwerpcyclus


### 1.1 Wat zijn drones?

Een drone is een onbemand voertuig dat je op afstand kunt bedienen of dat autonoom kan zijn. De taken van drones kunnen door menselijke interactie verstoord worden. Net als bij robots kunnen de taken al zo voorgeprogrammeerd zijn, dat ze alle taken automatisch uitvoeren. Als het voertuig geen motor heeft, zoals een zweefvliegtuig, dan is het geen drone.

Als je het over drones hebt, denkt iedereen aan een vliegende drone, maar er bestaan verschillende type drones voor verschillende terreinen, zoals de onderwater varende drone. Bekende drones zijn:

- Tello Edu (zie figuur 1.1): een eenvoudige vliegende drone;
- SeaFox AUV (zie figuur 1.2): deze drone kan onderwater varen.

In deze module zullen we ons beperken tot de vliegende drone.

### 1.2 Onderdelen van een drone

In de volgende hoofdstukken komt een aantal facetten van een drone aan bod. In elk hoofdstuk krijg je dus informatie die je kunt gebruiken in je eigen ontwerp.

Hoofdstuk 3-Besturingssysteem
Hoofdstuk 4 - Sensor
Hoofdstuk 5 - Vleugels of rotor
Hoofdstuk 6 - Romp
Hoofdstuk 7 - Aandrijving
Hieronder staat een korte toelichting bij elk onderdeel dat nodig is om een drone te bouwen.

Besturingssysteem: Als piloot van een drone heb je het liefst zoveel mogelijk controle. De drone heeft een flight controller, dit is het computersysteem van de drone. Met een afstandsbediening heb je volledige controle over de drone. Er zijn daarnaast ook mogelijkheden
om je drone zelfstandig op pad te sturen. Zo worden er drones geleverd met hun eigen applicatie waarmee je de drone naar eigen idee kunt programmeren. Ook zijn er drones beschikbaar die je te allen tijde kunt volgen. Hoofdstuk 3 gaat nader in op deze opties. Heeft je drone een full time operator nodig, of stuur je hem met de autopiloot op weg?

Sensor: Zonder accelerometer weet een drone niet of hij recht aan het vliegen is of niet. Dit is dus een belangrijke sensor voor een drone. Hoofdstuk 4 behandelt meerdere sensoren. Welke sensoren zet je in de drone en hoe sturen die hun data terug?

Vleugels of rotor: Je kunt kiezen voor vleugels (predator) of rotors (quadcopter). Deze keuze bepaalt mede de wendbaarheid van je drone. Daarnaast zijn meer aspecten van belang. Lange vleugels leiden tot meer liftkracht, maar ook tot meer luchtweerstand. Een drone met kleine vleugels moet de hele tijd op hoge snelheid vliegen om in de lucht te blijven. Het gaat hier dus o.a. om vliegduur, wendbaarheid en energieverbruik. Meer uitleg volgt in hoofdstuk 5.

Romp: De romp is de basis van een drone, ook wel het frame genoemd. De keuze voor de romp bepaalt grotendeels hoe je drone eruit komt te zien. Zo heb je de keuze in het aantal armen dat een romp heeft, hoe groot de romp wordt en van welk materiaal deze gemaakt is. Deze keuzes hebben invloed op de laadcapaciteit, het energieverbruik en de kosten van je drone. Verdere uitleg over de materiaalkeuze en de dikte van het gekozen materiaal volgt in hoofdstuk 6.

Aandrijving: De kracht om een vliegtuig aan te drijven kan op twee manieren worden geleverd: een motor die een propeller aandrijft of een straalmotor die een gasstroom genereert. Nadere toelichting staat in hoofdstuk 7. Kies je voor een propeller of een straalmotor? Hoeveel wil je er hebben? Wil je een batterij of een benzinetank? Deze keuzes bepalen voor een groot deel de operationele kosten. Hoe zwaar laat je de impact wegen van de keuze voor een energiebron op het milieu?

### 1.3 Ontwerpdossier

De module sluit je af met het ontwerpen van een drone aan de hand van de besproken casus. Daarbij is het belangrijk dat je na elk hoofdstuk goed kijkt naar wat je hebt geleerd, en hoe je dit kunt gebruiken voor je eigen ontwerp. Om dit materiaal bij te houden ga je werken met een ontwerpdossier. Daarin houd je het volgende bij:

- R\&D opdrachten
- Vliegende Rechter opdrachten
- Ontwerpproducten


### 1.4 Ontwerpcyclus

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-15.jpg?height=438&width=946&top_left_y=295&top_left_x=132)

Figuur 1.4 Ontwerpcyclus.

Om uiteindelijk tot een goed uitgewerkt ontwerp te komen, zul je eerst moeten kijken naar het begrip 'ontwerpen'. Een ontwerpopdracht kun je zien als het oplossen van een complex probleem. Je zult als team met veel verschillende factoren rekening moeten houden bij het ontwerpen van een drone.

In het ontwerpproces onderscheiden we zes fasen, zoals beschreven in figuur 1.4. Je zult daarin voortdurend moeten evalueren om te bepalen of je naar een eerdere stap in de ontwerpcyclus terug moet. Het proces is niet lineair. Voor de ontwerpopgave ga je al deze fasen langs. In dit hoofdstuk zul je vooral een begin maken met de fasen 1, 2 en 3.

## Fase 1. Analyseren \& beschrijven

Allereerst ga je kijken naar de ontwerpvraag. Wat wordt er nu verwacht? In het voorgaande hoofdstuk is de casus besproken. Je moet voor jezelf het ontwerpprobleem inzichtelijk maken. In de hoofdstukken 2 tot en met 7 krijg je telkens meer informatie aangereikt om je ontwerpprobleem op te lossen. Elke vraag/opdracht/theorie in deze module is onderdeel van deze fase.

## Fase 2. Programma van eisen (PvE) opstellen

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-15.jpg?height=912&width=746&top_left_y=1574&top_left_x=135)

Figuur 1.5 Morfologische kaart van een fiets

Waaraan moet het ontwerp voldoen? Denk aan vorm, materiaal, eisen, wensen, sterkte, gebruikersgroep. Vooraf stel je een programma van eisen op aan de hand van eisen/wensen van het comité (Casus), wettelijke eisen, maar ook eisen/wensen die jullie zelf belangrijk vinden. Zodra je een ontwerp(schets) hebt gemaakt, kun je aan de hand van je PvE testen of het ontwerp voldoet aan de vooraf gestelde eisen. Dit programma van eisen moet je zien als ontwikkeldocument. In hoofdstukken 2 tot en met 7 zul je veel informatie aangereikt krijgen, waarmee je het ontwikkeldocument mogelijk wilt herzien. Je kunt op dat moment het PvE aanpassen of aanvullen.

## Fase 3. Ideeën bedenken

Er zijn veel verschillende manieren op ideeën te bedenken. Om een overzicht te krijgen van de mogelijkheden maken jullie gebruik van een morfologische kaart, zie figuur 1.5. Een morfologische kaart geeft een overzicht van de ontwerpopties per onderdeel van een drone, in jullie geval is dit de winkel met drone onderdelen. Deze winkel beheert je docent. Gedurende de module krijgen jullie steeds meer informatie aan punten die je kunt inzetten in

Dit zorgt ervoor dat je richting het einde van de module beter start aan de eindontwerp-fase.

In hoofdstuk 9 krijg je nadere toelichting over de fasen $3 \mathrm{t} / \mathrm{m} 6$.

## Opdracht: Ontwerpcyclus fase 1 en 2

Om tot een goed ontwerp te komen zul je de verschillende fasen van een ontwerpcyclus moeten doorlopen. Voor deze opdracht ga je werken aan de fasen 1 en 2 . Zoals de naam cyclus al aangeeft zul je hier meerdere keren op terug moeten kijken.

Fase 1: Om het ontwerpprobleem inzichtelijk te maken, maak je gebruik van een woordweb (zie figuur 1.6). Daarin zet je de centrale ontwerpvraag (casus) in het midden van het blad. Bedenk wat er allemaal komt kijken bij deze casus. Daarin kun je ook inzichtelijk maken wie er met het probleem te maken heeft en wat voor type drones je verwacht nodig te hebben. Zoek ook onderlinge verbanden.

Fase 2: Zoals in fase 2 al is uitgelegd, ga je nu een programma van eisen opstellen. Je kunt gebruik maken van je zelfgemaakte woordweb in fase 1 en de besproken casus in het vorige hoofdstuk. Maak duidelijk onderscheid tussen eisen die het comité stelt, en die jullie zelf belangrijk vinden.

## Maak en lever in:

R\&D 1a Een woordweb waarin je de casus analyseert
R\&D 1b Een eerste opzet van het PvE

## Beloning:

Het goed uitvoeren van deze opdracht levert algemene R\&D-punten op die je later in je voordeel kunt gebruiken.

## Leerdoelen

Na dit hoofdstuk kun je:

- verschillende onderdelen van een drone benoemen;
- de fasen van een ontwerpcyclus benoemen;
- een woordweb maken;
- een programma van eisen opstellen;
- een morfologische kaart opzetten.


## 2 Geschiedenis en maatschappij

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-17.jpg?height=449&width=606&top_left_y=752&top_left_x=128)

Figuur 2.1 Winston Churchill en anderen wachten op de lancering van een doelwit-drone van de Havilland Queen Bee, 6 juni 1941.

Drones bestaan al meer dan honderd jaar. Het waren niet de drones die we nu kennen, maar onbemande luchtvaartuigen. Sinds de uitvinding van drones zijn ze gebruikt voor verschillende doeleinden. In dit hoofdstuk krijg je informatie over de geschiedenis van drones en over de invloed van drones op onze maatschappij.

### 2.1 Geschiedenis van de drone

Drones zijn uitgevonden om zonder personeel een gebied aan te vallen of te verdedigen. Deze briljante uitvinding was voornamelijk bedoeld voor militaire doeleinden, met de intentie om het leven van militairen te sparen. Pioniers in deze uitvinding waren de Oostenrijkers, Duitsers (uit toenmalig Nazi-Duitsland) en Amerikanen.

Het eerste gebruik van een drone vond plaats in 1849 door Oostenrijk. Zij stuurden onbemande, met bommen gevulde ballonen naar Venetië om die stad aan te vallen. Innovatie van drones begon in de vroege jaren 1900. Drones werden vanaf toen ook gebruikt als oefendoelwit voor het trainen van militair personeel. Er was veel vooruitgang in de ontwikkeling van drones tijdens de Eerste en Tweede Wereldoorlog. De eerste onbemande vliegtuigen werden gebouwd tijdens de Eerste Wereldoorlog. Deze drones werden gelanceerd door een katapult of werden gevlogen met behulp van radiobesturing (zie figuur 2.1).

Het eerste geschaalde, op afstand bestuurde voertuig werd ontwikkeld door filmster en model-vliegtuigenthousiasteling Reginald Denny in 1935. Tijdens de Tweede Wereldoorlog gebruikte men drones om luchtdoelgeschut te trainen en om missies te vliegen. In 1955 gebruikte de Amerikaanse landmacht het model 1001, dit was een op afstand bestuurbaar vliegtuig. Camera's op de drones zijn geïntroduceerd in het begin van de jaren ' 70 om het land te bespioneren. De eerste drone die voorzien was met wapens was de Predator MQ-1 in 1994.

De meest gebruikte afkorting voor de vliegende drone is UAV, deze afkorting staat voor Unmanned Aerial Vehicle (vertaling: onbemand luchtvaartuig). De vliegende drone is het meest bekende type drone en het meest ontwikkeld op dit moment, maar wetenschappers besteden de laatste jaren aandacht aan het ontwikkelen en verbeteren van andere type drones. Onderwaterdrones zijn sinds 2001 in ontwikkeling om zeemijnen te bestrijden, zoals de SeaFox AUV (zie figuur 1.2, blz 12). De nieuwste onderwaterdrones worden gebruikt om foto's en videomateriaal onder water te maken.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-18.jpg?height=429&width=572&top_left_y=348&top_left_x=131)

Figuur 2.2 Drone met camera
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-18.jpg?height=1093&width=576&top_left_y=993&top_left_x=106)

Figuur 2.3 Drie voorbeelden van drones die in de oorlog in Ukraine gebruikt worden. Van boven naar beneden, de "Baba Yaga" hexacopter voor zware lasten, de HESA Shahed 136 voor lange afstanden de DJI Mavic quadcopter voor observatie van de frontlinie.

### 2.2 Drones in onze maatschappij

De populariteit van drones neemt toe, vooral omdat ze kleiner en betaalbaarder zijn geworden. Op dit moment zetten we drones in bij oorlogen, voor professionele (commerciële) doeleinden en als hobby.

Veel televisiemaatschappijen en makelaars maken gebruik van drones om opnames te maken die ze voor commerciële doeleinden kunnen gebruiken. Drones die ingezet worden om een landschap op te nemen beschikken momenteel niet alleen over een hoge resolutie camera (zie figuur 2.2), maar ook over sensoren om obstakels te kunnen detecteren. Deze drone kan dus zelf obstakels ontwijken zonder dat de bestuurder daar alert op hoeft te zijn.

In 2020 hadden drones een beslissende invloed op het verloop van een oorlog. In het conflict tussen het Armeense en Azerbeidjaanse leger werd op grote schaal Armeens materieel uitgeschakeld door militaire drones van Turkse en Israëlische makelij.

In de oorlog in Ukraine worden naast militaire drones op grote schaal goedkope commercieel verkrijgbare drones gebruikt. Er zijn schattingen dat er geregeld zo'n tienduizend drones boven de frontlinies vliegen die vaak maar enkele dagen meegaan. Deze kleine drones observeren met camera's de gehele frontlinie, waardoor het heel lastig is geworden om troepen te verzamelen en of aanvallen uit te voeren. Spectaculair zijn de video's op YouTube die laten zien zijn hoe kleine commercieel verkrijgbare FPV (First Person View) racedrones dure zware gevechtstanks uitschakelen.

In de loop van de oorlog zijn er tientallen bedrijven betrokken geraakt bij de massaproductie van drones ten behoeve van de oorlogsvoering. De Oekraïense regering heeft het "Leger van Drones" project opgezet om per jaar honderdduizenden drones aan te kunnen schaffen. Het doel is om met grote aantallen, relatief goedkope drones, tegenwicht te bieden aan het zware materieel van het veel grotere Russische Leger. In 2023 heeft de regering verschillende wedstrijden voor drone ontwerpers georganiseerd waarin tientallen droneontwerpers meedoen in ontwerp wedstrijden van gesimuleerde aanvallen. Uit zo'n wedstrijd is bijvoorbeeld de succesvolle "Baba Yaga" hexacopter ontstaan. Een drone die meer dan 20 kg kan vervoeren.

Ook het Russische leger gebruikt veel drones. Een voorbeeld is de Iraanse HESA Shahed 136 kamikaze drone die met zijn vleugels en verbrandingsmotor meer dan 1000 km ver kan vliegen.

Op 13 oktober 2022, vond het eerste geregistreerde luchtgevecht tussen drones plaats. Een Oekrainse DJI Mavic quadcopter ramde een Russische drone van het zelfde model welke vervolgens neerstortte.

Hobby drones zijn heel leuk om te hebben of als cadeau te geven. Ze verschillen in kwaliteit en in prijs. Je moet er wel op letten dat je niet overal met je drone mag vliegen, in gebieden rondom vliegvelden is dit bijvoorbeeld verboden. Drones mag je alleen in het vrije deel
van het luchtruim gebruiken. In de Bronnen tref je een link van een kaart aan waarop is aangegeven waar je een drone wel of niet mag vliegen (de Drone no fly zone in Nederland).

Om drones te vliegen in onze luchtruim heb je een vliegvaardigheidsbrevet nodig. Zie verder in Hoofdstuk 8.

## Vragen en opdrachten

1. Over drones
a. Geef in eigen woorden weer wat een drone is.
b. Wat is het verschil tussen een drone en zweefvliegtuig?
c. Leg uit of de poppetjes van een draaiorgel ook robots zijn.
d. Noem twee type drones die op verschillende terreinen bediend kunnen worden.
2. Over de geschiedenis van de drone
a. Wat is de voornaamste reden waarom drones zijn uitgevonden en wie waren de pioniers hierin?
b. Wanneer en waarvoor is voor het eerst een drone gebruikt?
c. Wat betekent UAV?
3. Over de toepassing van drones in onze maatschappij Waarvoor zou je een drone kunnen gebruiken? Beschrijf ten minste twee situaties waarvoor een drone gebruikt kan worden.

## (optioneel) Extra opdracht

Een drone is iets leuks om te hebben. Helaas mag je niet overal een drone vliegen. De overheid heeft een aantal regels hiervoor bepaald die elke drone eigenaar moet weten. Ga naar de website:
https://www.rijksoverheid.nl/onderwerpen/drone/regels-hobbydrone en beantwoord de volgende vragen:

- Tot welke hoogte kun je een drone vliegen?
- Mag je een drone overal vliegen?
- Mag je een drone in het donker vliegen?
- Is het toegestaan om overal filmen en foto's te maken met een drone?


## Opdracht: Type drones

Elk jaar komen er nieuwe drones op de markt. Deze drones kunnen in allerlei gebieden ingezet worden. Onderzoek welke type drones er op dit moment bestaan. Beschrijf van minimaal 3 verschillende type drones waarvoor ze gebruikt worden en benoem de eigenschappen van deze drones.

Hint: Gebruik het zoekwoord "latest drones" in een zoekmachine of YouTube

## Maak en lever in:

R\&D 2 Een verslag van 1 pagina waar je ten minste 3 verschillende type drones beschrijft en hun eigenschappen.

## Beloning:

Het goed uitvoeren van deze opdracht levert één algemene R\&D-punt op die je later in je voordeel kunt gebruiken.

## Leerdoelen

Na dit hoofdstuk kun je:

- de reden benoemen waarom drones zijn uitgevonden;
- situaties benoemen waarvoor je een drone kunt inzetten;
- verklaren waarom het belang van het ontwerpen van drones de laatste jaren is toegenomen;
- (extra) de regels voor recreatief gebruik van drones benoemen.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-21.jpg?height=209&width=393&top_left_y=227&top_left_x=289)
an BUSIIIESS.
Drone hits passenger plane in Canada
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-21.jpg?height=321&width=567&top_left_y=636&top_left_x=122)

CNN nieuwsbericht over het incident

## De Vliegende Rechter

Een drone is op een vliegtuig geknald bij een vliegveld in het Canadese Quebec. Er vielen geen gewonden.

Het drone-ongeluk vond donderdag plaats, zo maakte de Canadese minister van transport Marc Garneau zondagavond bekend. Er vielen geen gewonden bij de botsing tussen de drone en een vliegtuig van Skyjet Aviation op de luchthaven Jean Lesage. Het vliegtuig, met acht personen aan boord, liep volgens Garneau 'lichte schade op' en kon veilig landen.
Bron: bright.nl, zondag 15 oktober 2017

## Wat denkt de Vliegende Rechter?

VR2 Drones op het vliegveld
a. Noem drie problemen die drones kunnen veroorzaken op een luchthaven.
b. Er is uiteraard al één en ander geregeld over het gebruik van drones rondom luchthavens. Beschrijf kort welke problemen jij ziet bij het handhaven van die regels.
c. Beschrijf wat jij als drone-ontwerper hieraan zou kunnen of moeten doen.

Betrek ook botsingen met vogels in het nadenken over deze casus. Vogels en drones kunnen beide rondhangen op vliegvelden.
d. Wat is het verschil tussen het vermijden van risico's door de vogels en door drones?

## 3 Besturingssysteem van drones

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-22.jpg?height=1049&width=487&top_left_y=521&top_left_x=199)

Figuur 3.1 Het besturingssysteem van een smartphone
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-22.jpg?height=480&width=487&top_left_y=1893&top_left_x=185)

Figuur 3.2 Logo van ROS

Net als je smartphone en je computer hebben tv's, auto's, horloges en vrijwel alle andere apparaten die 'smart' kunnen zijn, een eigen besturingssysteem. Drones hebben ook zo'n besturingssysteem.

### 3.1 Besturingssysteem

Een besturingssysteem is de programmatuur die de hardware en de andere software op een apparaat aanstuurt. Zonder het besturingssysteem zou je niet alle hardware kunnen gebruiken die je apparaat bezit.

Alle computers en overige apparaten die een computerachtig systeem hebben, zoals laptop, desktop, smartphone en robot hebben een besturingssysteem. In Nederland gebruiken we meestal de Engelse naam voor besturingssysteem: operating system, afgekort OS.

## Hardware

De fysieke onderdelen van een apparaat of machine zoals computer, mobile telefoon of robot. Voorbeelden van computer hardware zijn toetsenbord, geheugen, muis en moederbord.

## Software

Alle programma's en instructies die bepalen hoe een apparaat in dit geval computer en robot moet werken.

## Een voorbeeld

Je opent Google Chrome op je smartphone via de knop "Google Chrome" die op je scherm wordt weergegeven dankzij het besturingssysteem. Het besturingssysteem opent Google Chrome en laadt het in het werkgeheugen, zodat dit programma kan gaan draaien. Wanneer Google Chrome een website wil weergeven, zal het aan het besturingssysteem vragen via welke verbinding hij contact kan maken met het internet. Daarna wordt de website opgehaald en via Google Chrome zal het besturingssysteem de website weergeven.

### 3.2 ROS

Robots hebben een eigen besturingssysteem: ROS, robot operating system. Dit is een open source programma om robots dingen te laten doen. ROS is ontworpen als een gemeenschappelijk softwareplatform voor mensen die robots, zoals drones, bouwen en gebruiken.

## Open source software

De software waarvan de (bron)code voor iedereen beschikbaar is en aangepast en verspreid mag worden.

ROS is geen traditioneel besturingssysteem zoals Windows, Linux of IOS. Het is als een verzameling bibliotheken, algoritmen en hulpmiddelen die je kunt gebruiken om je robot te laten functioneren. Door middel van ROS maak je je robot krachtiger.

## Algoritme

Een algoritme is een stappenplan dat bij een probleem doorlopen kan worden om de oplossing te krijgen. Net zoiets als een recept voor een appeltaart. Vaak met behulp van een diagram, zie vraag 10.

## ROS-onderdelen

ROS bestaat uit verschillende onderdelen.

- Ten eerste is het een set van stuurprogramma's waarmee je gegevens van sensoren kunt lezen en opdrachten naar de motoren en andere onderdelen van de robot kunt sturen. ROS ondersteunt de meeste populaire hardware, waaronder veel commerciële robot/drone-systemen.
- Verder is er in ROS ook een aantal essentiële algoritmen voor robotica aanwezig waarmee je de wereld in kaart brengt en er doorheen kunt navigeren. Onder essentiële algoritmen verstaan we stukjes code voor bijvoorbeeld sturen van bewegingen.
- Met ROS kun je sensorgegevens weergeven en deze gegevens interpreteren en kun je bewegingen plannen, objecten analyseren en nog veel meer andere dingen. ROS is erg populair in de robotica-wereld en er zijn in ROS veel geavanceerde algoritmen, zoals het vinden van een landingsplaats naar aanleiding van een foto, beschikbaar. In ROS zit de hele computerinfrastructuur waarmee je de gegevens van je robot(s) kunt verbinden met een complex robotsysteem en waar je je eigen algoritmen aan kunt toevoegen.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-23.jpg?height=475&width=723&top_left_y=1978&top_left_x=107)

Figuur 3.3 ROS-Diagram

- In ROS kun je een groot aantal hulpprogramma's vinden waarmee je op een simpele manier de status van de robot (of hij vliegt, hoe het met zijn batterijen is of welke richting hij op gaat) en van de algoritmen zichtbaar kunt maken, fouten kunt opsporen en meetgegevens kunt vastleggen. Het "debuggen" van robotsoftware heeft speciale uitdagingen en deze grote verzameling van hulpprogramma's is een van de onderdelen die ROS zo krachtig en succesvol maken.
Ten slotte is ROS uitgebreid gedocumenteerd, zoals in http://wiki.ros.org, die veel aspecten van het systeem documenteert en een vraag-en-antwoord-site waar je zowel om hulp kunt vragen als informatie kunt delen over wat je hebt geleerd, verbeterd of nieuw ontwikkeld.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-24.jpg?height=244&width=456&top_left_y=289&top_left_x=203)

Figuur 3.4 AR. Drone

## ROS-ondersteunend platform

Er zijn verschillende ondersteunende ROS-platformen door de community van robotonderzoekers en drones ontwerpers.

We behandelen in dit hoofdstuk een systeem voor autonome navigatie (zelfrijdend systeem) van de 'AR. Drone' met minimale hardware- en software-toevoegingen. Dit model drone, de AR. Drone, is ontwikkeld door het Franse bedrijf Parrot in 2010. De AR. Drone is ontworpen om te worden bestuurd door mobiele of tablet-besturingssystemen (zoals iOS of Android).

### 3.3 Hardware vereist voor het platform

Deze drone heeft twee elektrische boards. Het belangrijkste board van de AR. Drone (moederboard) bevat een processor met een snelheid van 468 MHz tot $1 \mathrm{GHz}^{*}$, twee camera's, een wifi-module en een USB-connector om de programma's te uploaden en software te debuggen. De twee camera's hebben verschillende functies. De ene is verticaal georiënteerd, wijst naar de grond, heeft een openingshoek van $63^{\circ}$ (zie figuur 3.5) en een framesnelheid van 60 frames per seconde (fps). Deze camera wordt gebruikt om de horizontale snelheid van het voertuig te schatten en daarom hoeft de hoek niet groter te zijn. De tweede camera wijst naar voren en moet een breder beeld hebben om de obstakels waar te kunnen nemen. Daarom heeft deze camera een openingshoek van $93^{\circ}$ en een beeldsnelheid van 15 tot 30 fps . Beide camera's kunnen worden gebruikt voor het detecteren van bijvoorbeeld de aanwezigheid van andere drones.

Het navigatieboard bevat alle sensoren die nodig zijn voor het schatten van de toestand van de drone.

## hertz (Hz)

is de eenheid van de frequentie
$1 \mathrm{GHz}=1000 \mathrm{MHz}$
$1 \mathrm{MHz}=1000 \mathrm{kHz}$
$1 \mathrm{kHz}=1000 \mathrm{~Hz}$

### 3.4 Softwarecomponenten

Het besturingssysteem van een drone bestaat uit twee hoofdonderdelen: een externe verwerkingseenheid en een proxyprogramma dat fungeert als een brug tussen de drone en de externe verwerkingseenheid.

Het proxy-programma draait op de drone en maakt uitwisseling van informatie met de externe verwerkingseenheid mogelijk. Je kunt (zeer) complexe taken (bijvoorbeeld het meten van de afstand met de grond) voor navigatie en besturing uitvoeren in de externe verwerkingseenheid. De externe verwerkingseenheid kan communiceren met verschillende sensoren. Een optioneel basisstation communiceert met de externe verwerkingseenheid om de vluchtgegevens te configureren.

De drone kan heel veel sensorgegevens aan de bestuurder leveren. Deze gegevens komen via twee verschillende soorten streams:

- Een Navdata-stream met gegevens over de status van het voertuig. De navigatiegegevens (navdata) gaan over de status en veiligheid van de motoren, vleugels, sensoren en camera's en ook de communicatie tussen hen. Een deel van navdata gaat ook over bewegingen van de drone, snelheid, de afstand met de obstakels en met de grond op basis van visuele informatie. Bewegingen die voorkomen zijn: slingeren of de rol (draaien om de horizontale as in de vliegrichting), stampen of de pitch (draaien om de horizontale as dwars op de vliegrichting) en gieren of de yaw (draaien om de verticale as).

De visuele informatie bevat alle gegevens die de drones door de camera's en sensoren kunnen verzamelen. Die gegevens worden verstuurd naar de externe verwerkingseenheid om de drone een compleet overzicht van zijn omgeving te geven en om veilig te kunnen vliegen.

- Een videostream die de gecodeerde video van de camera's verstuurt naar de externe verwerkingseenheid. Als je een foto of video wilt maken met je drone, voert het besturingssysteem de videostream-algoritme uit. Je kunt dan bepalen welke camera moet functioneren. En dan wordt de foto of video gecodeerd naar binaire getalen door het besturingssysteem. Vervolgens kun je je foto of video opslaan in het geheugen.

De processor draait op een embedded (ingebed) Linuxbesturingssysteem dat tegelijkertijd de draadloze communicatie, het schatten van de traagheidsstatus en de regelalgoritmen beheert.

## Binaire code

Een systeemcodering met slechts twee symbolen 0 en 1 . In een computer en andere digitale apparaten moeten alle gegevens zoals tekst, foto en video worden gecodeerd naar binaire codes.

Belangrijk voor drones is dat de drone gegarandeerd binnen een bepaalde tijd kan reageren op sensor input. Het gaat er vooral om dat de actie op tijd komt en dat betekent niet perse dat het om snelheid gaat.

Een speciaal soort besturingssystemen dat zijn de real-time systemen, zoals bijvoorbeeld Paparazzi. Die zijn niet per se snel, maar ze kunnen wel gegarandeerd binnen een bepaalde tijd resultaat leveren. Operating systemen zoals Windows en Linux zijn niet realtime. Dat betekent dat ze hoewel ze meestal erg snel reageren, soms, doordat ze bezig zijn met een andere taak, een urgente beslissing te laat nemen. Snellere computers zijn vaker op tijd, maar er is geen garantie als het operating system niet real-time is.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-26.jpg?height=958&width=635&top_left_y=435&top_left_x=88)

Figuur 3.6 Softwarecomponenten, gekoppeld aan camera's en sensoren.

### 3.5 Autopiloot en Drones

De drone is geclassificeerd als onbemand luchtvaartuig (UAV), en daarom is de verwachting dat in de toekomst alle drones met een autonoom besturingssysteem zullen worden uitgerust.

Zelfbesturende drones maken dus deel uit van onze toekomst. In het laatste decennium zijn er om (nationale) veiligheidsredenen veel pogingen ondernomen dit soort drones te ontwikkelen. Veel robotonderzoekers worstelen met de gecompliceerde structuur ervan en er wordt veel geld uitgegeven voor onderzoek in dit domein.

De software voor autonoom vliegen en opdrachten uitvoeren draait op een microcontroller*. Deze bestaat uit drie onderdelen:

- positiebepaling
- routeplanning
- besturing

Het eerste onderdeel gebruikt positieschattingen van de drone met visie-algoritmen. De positie en koers worden in wereldcoördinaten gegeven. Het proxy-programma haalt deze gegevens uit de navigatiegegevens van de drone die worden verzameld door de camera's en sensoren. Vervolgens stuurt hij een binair bericht naar de microcontroller met de status, de positie en de richting van de drone. Je kunt de drone als een extra sensor zien die positie-informatie doorgeeft aan de plannings- en besturingsmodules die op de microcontroller worden uitgevoerd.

Het tweede onderdeel, de routeplanning, berekent een traject voor de drone dat moet worden afgelegd op basis van vooraf gedefinieerde vormen of door de gebruiker gedefinieerde waypoints (waypoint = een plaats op een route waarop de koers wordt gewijzigd). Met wiskundige berekeningen kun je een vooraf gedefinieerde vorm, zoals een eenvoudige rechte lijn, een cirkel of een achtvorm laten volgen. Om waypoints te volgen bepaal je een reeks coördinaten die een gewenst traject beschrijven.

Elk waypoint $w$ is gedefinieerd als een triplet $w=[x, y, z]$ waarbij $x$, $y$, $z$ wereldcoördinaten zijn met als oorsprong de startlocatie van de drone. Het traject wordt berekend als een reeks van met elkaar verbonden functies van tijd voor elk van de assen. Op deze manier navigeren, zorgt ervoor dat de camera altijd in de vliegrichting staat, maar het is niet optimaal voor de bediening van de drone.

In het kort, vliegt een drone zelfstandig met behulp van het besturingssysteem dat een algoritme uitvoert. Op basis van het algoritme vliegt de drone volgens de waypoints die door camera's en sensoren verstuurd worden. Hij detecteert elk moment de nieuwe waypoint en volgt die tot de bestemming.

## Microcontroller

Een kleine computer dat een apparaat kan besturen.

## Vragen en opdrachten

4. Waarom moet je eigenlijk een apart besturingssysteem voor robots maken? Kun je dat niet gewoon met Windows, Linux of desnoods Android?
5. Je opent de website van bijvoorbeeld de NS via Google Chrome. Leg de rol van het besturingssysteem in dit proces uit.
6. Waarom is ROS open source? De makers zouden er toch veel geld aan kunnen verdienen? (Zoek op internet de informatie over Open source software)
7. De drone heeft een camera met openingshoek van $63^{\circ}$ en een camera met openingshoek van $93^{\circ}$. Leg uit waarom er een verschil is tussen de openingshoek van camera's.
8. Je wilt graag een nieuw algoritme uploaden op je eigen drone.
a. Hoe kun je dit doen en met welke van de hardware onderdelen van de drone doe je dat?
b. Welk programma helpt je om het algoritme bekend te maken voor je drone?
9. Leg het proces van het besturingssysteem van de drone uit als de drone een nieuwe foto gaat maken.
10. Hiernaast (in figuur 3.7) zie je een deel van het algoritme van opdracht 9 in een diagram. Maak het diagram af dat het hele proces van opdracht 9 laat zien.
11. In de tekst staat: "Een deel van navdata gaat ook over bewegingen van de drone, snelheid, afstand met de obstakels en grond op basis van visuele informatie". Wat is visuele informatie?
12. a .Welke taken kun je uitvoeren in een externe verwerkingseenheid?
b. Heb je een real-time system nodig voor navigeren?
13. Een foto moet gecodeerd worden naar binaire code. Vertel hoe en waarom.
14. Bedenk enkele redenen waarom je zelfsturende drones bouwt.
15. De software voor autonome drones draait op een microcontroller. De microcontroller bestaat uit drie onderdelen. Noem en leg deze 3 uit.
16. Leg in het kort uit hoe een drone zelfstandig kunt vliegen.

Opdracht: Algoritme
Hiernaast zie je het algoritme voor het detecteren van een landingsplaats voor de drone. Eerst maakt de camera een foto en stuurt deze naar het besturingssysteem.
Vervolgens wordt de foto geconverteerd naar een binaire code (0 en 1). Als de code van de foto hetzelfde is als de code van de landingsplaats, wordt de plaats gedetecteerd.

Teken nu zelf een algoritme/diagram dat een drone zelfstandig naar links kan laten gaan.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-28.jpg?height=867&width=540&top_left_y=269&top_left_x=1309)

Figuur 3.8 Het algoritme voor het detecteren van de landingsplaats

Maak en lever in:
R\&D 3 Het algoritme/diagram dat je gemaakt hebt.

## Beloning:

Het goed uitvoeren van deze opdracht levert R\&D-punten op die gebruikt kunnen worden voor het ontwerp van het besturingssysteem

## Leerdoelen

Na dit hoofdstuk kun je:

- het besturingssysteem van de drones herkennen;
- onderdelen van ROS benoemen;
- een ROS-diagram tekenen;
- de vereiste hardwarecomponenten en hun functies herkennen;
- softwarecomponenten van een ROS benoemen;
- uitleggen wat visuele informatie is;
- uitleggen waarvoor een real-time system bij een drone nodig
- de onderdelen van autopilot software benoemen en de functie van elke component beschrijven;
- uitleggen wat een waypoint is;
- het autonome proces van een drone en de rol van de programma's toelichten;
- enkele algoritmen van autopilot beschrijven.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-29.jpg?height=1266&width=595&top_left_y=189&top_left_x=142)

Figuur 3.9 Huishoudrobot, 2008

## De Vliegende Rechter

## Robots die raad weten met morele dilemma's

Specialisten experimenteren met robots die zelfstandig ethische keuzen kunnen maken. Zijn dit geprogrammeerde 'ethische zombies' of leren ze telkens bij?

De razendsnel ontwikkelende technologie laat weinig aan de verbeelding over. Nieuwe, zelflerende software: eind mei 2017 versloeg Google' s computerprogramma AlphaGo weer een wereldkampioen in het voor computers ooit onbereikbare bordspel Go. Zowel fysieke robots als computers worden steeds beter en zelfstandiger.
De actieradius van robots beperkt zich allang niet meer tot een gecontroleerde omgeving zoals een fabriek. Bij zelfrijdende auto's en zorgrobots moet je rekening gaan houden met computergestuurde machines die tussen en met mensen werken.

Hoe veilig is dat? Je wilt niet dat je zorgrobot per ongeluk je zoontje van de trap gooit omdat zijn software hem opdraagt exact om drie uur de was te doen.
Bron: NRC, 3 november 2017

## Wat denkt de Vliegende Rechter?

## VR3 Asimovs regels

Hoe voorkom je dat intelligente robots zich tegen de mensheid keren? Hier dacht de Amerikaanse schrijver Isaac Asimov in 1942 al over na. In zijn sciencefiction boeken loste hij dit probleem op door elke robot drie gedragsregels mee te geven.
a. Zoek die gedragsregels op en noteer ze.
b. Noem drie problemen die kunnen voorkomen met een zelfstandig functionerende huishoudrobot.
c. Beschrijf wat jij als drone-ontwerper hiervan zou kunnen leren of hiermee zou moeten doen. Bedenk daarbij drie voordelen wanneer de apparaten om ons heen slimmer worden.
d. Waarom zouden we autonome robots niet vertrouwen terwijl wij al sinds de geschiedenis van de mensheid autonome dieren vertrouwen?
e. Waarom houden mensen zich niet aan Asimov's $1^{e}$ en $3^{e}$ wet? En gaat de $2^{\mathrm{e}}$ wet nu over het gedrag van de robot of het gedrag van de mens? (waarbij de robot dan toch een oordeel velt over het gedrag van de mensen)
f. Waarom zou een robot die intelligenter is dan mensen net zo een kwaadaardige inborst hebben als mensen? Oorlog voeren is heel dom en slecht voor het milieu.
g. Waarom zou een autonome auto zich uiteindelijk niet gewoon moeten gedragen als een verbeterd paard? Op een paard kan ik dronken veilig thuiskomen. Waarom zou dat niet met een autonome auto kunnen? Die weet meer van de weg en de verkeersregels en heeft meer/betere (?) sensoren dan een paard.

## 4 Dataverzameling, snelheids- en plaatsbepaling

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-30.jpg?height=464&width=595&top_left_y=542&top_left_x=88)

Figuur 4.1 Is de bemanning van deze helikopter echt nodig?
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-30.jpg?height=592&width=452&top_left_y=1189&top_left_x=177)

Figuur 4.2 Gyroscoop
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-30.jpg?height=369&width=500&top_left_y=2100&top_left_x=127)

Figuur 4.3 De MMA8452Q versnellingsmeter

Als een drone een bosbrand moet signaleren, wil de brandweer weten wat de plaats is van de brand om die te kunnen blussen. Hiervoor moet de drone dus kunnen bepalen waar hij is, maar hoe doet hij dat? Ook is het belangrijk voor een drone om te "weten" wanneer hij scheef hangt of wanneer hij dreigt te kantelen. Als de drone dit niet weet, kan hij neerstorten. In deze paragraaf ga je kijken naar het systeem dat voor oriëntatie, snelheids- en plaatsbepaling zorgt.

### 4.1 Oriëntatie

Het veelgebruikte apparaat om oriëntatie te bepalen is de gyroscoop. Een gyroscoop is een vrij eenvoudig apparaat waarbij een wiel vrij kan ronddraaien in alle richtingen (zie figuur 4.2). Toch zijn de eigenschappen van een gyroscoop niet eenvoudig. Er is veel kracht nodig om de richting van het draaiende wiel te veranderen. Het wiel draait dus niet mee met de draaiing van zijn frame. Omdat het frame wel draait en het wiel niet, kun je door het verschil te meten de hoek bepalen waaronder het frame en dus de drone zicht bevindt.

### 4.2 Snelheids- en plaatsbepaling

Drones gebruiken versnellingsmeters om uit de gemeten versnelling de snelheid en de plaats te kunnen berekenen. De drone verzamelt dus de juiste data en rekent ermee. De manier waarop dit gebeurt, lijkt sterk op wat je bij het vak natuurkunde hebt geleerd bij modelleren.

De versnellingsmeter geeft een versnelling $a$ (in $\mathrm{m} / \mathrm{s}^{2}$ ) aan. Dit is de verandering van snelheid in de tijd. De snelheid berekent de drone als volgt: de verandering van snelheid wordt bij de huidige snelheid opgeteld. Per meetpunt van de versnellingssensor wordt de snelheid aangepast. De formule die de drone hiervoor gebruikt is:

$$
v=v_{0}+a \cdot \Delta t
$$

Hierin is $v$ de eindsnelheid, $v_{0}$ de beginsnelheid en $\Delta t$ de tijd van de tijdstap waarvoor de versnelling $a$ geldt.
De plaats wordt op een vergelijkbare manier bepaald als de snelheid. Hierbij maak je gebruik van het feit dat de afgelegde afstand gelijk is aan de snelheid maal de tijd (mits die tijd $\Delta t$ kort is). De volgende formule gebruikt de drone daarbij:

$$
s=s_{0}+v \cdot \Delta t
$$

Hierin is $s$ de totaal afgelegde afstand, $s_{0}$ de al afgelegde afstand en $\Delta t$ de tijdstap waarvoor de snelheid $v$ geldt.

## Voorbeeld 1

Een quadcopter is opgestegen en gaat over het schoolplein vliegen. Zijn snelheid parallel aan het schoolplein is $1,00 \mathrm{~m} / \mathrm{s}$. De quadcopter gaat versnellen. De versnellingsmeter van de quadcopter meet 50 keer per seconde zijn versnelling. De meetwaarden in $\mathrm{m} / \mathrm{s}^{2}$ zijn: 1,2; 1,3; 1,5; 1,4; 1,4 (in chronologische volgorde).
a Bereken de eindsnelheid van de drone.
b Bereken de afstand die de quadcopter heeft afgelegd voor het behalen van de eindsnelheid.
a De tijdstap is $1 / 50=0,020 \mathrm{~s} . \mathrm{Na} 0,020 \mathrm{~s}$ is de snelheid dus:
$v=v_{0}+a \cdot \Delta t=1,00+1,2 \times 0,020=1,024 \mathrm{~m} / \mathrm{s}$.
Op eenzelfde manier bereken je de eindsnelheid:
$v=1,024+1,3 \times 0,020+1,5 \times 0,020+1,4 \times 0,020+1,4 \times 0,020=$ $1,136 \mathrm{~m} / \mathrm{s}$
b Eerst moet je de snelheid op elk meetpunt weten. Volgens de formule $v=v_{0}+a \cdot \Delta t$ kom je uit op de volgende snelheden bij de meetpunten in $\mathrm{m} / \mathrm{s}: 1,00 ; 1,024 ; 1,05 ; 1,08 ; 1,108 ; 1,136$. Voor de afgelegde afstand gebruik je dan $s=s_{0}+v \cdot \Delta t=$ $=0+1,00 \times 0,020+1,024 \times 0,020+1,05 \times 0,020+1,08 \times 0,02+$ $+1,108 \times 0,020+1,136 \times 0,020=0,128 \mathrm{~m}$

Zoals uit de voorbeeldvragen blijkt, komt er veel rekenwerk kijken bij het gebruik maken van hele kleine tijdstapjes. Dit met de hand uitrekenen kost veel tijd. Bij drones gebeurt het rekenen natuurlijk digitaal, daarom bepaal je in de R\&D opdracht de plaats met Coach. Coach is een computerprogramma dat o.a. met data kan rekenen en de uitkomsten overzichtelijk kan weergeven. De bovenstaande theorie vormt de basis voor de instructie die je Coach moet voorschrijven om de data juist te verwerken.

## Nauwkeurigheid

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-31.jpg?height=415&width=621&top_left_y=1894&top_left_x=112)

Figuur4.4 Een kleine afwijking in de plaats kan grote gevolgen hebben.

Bovenstaande methode is geen perfecte methode. Het is een benadering van de werkelijkheid. De methode gaat er namelijk van uit dat gedurende de gehele tijd $\Delta t$ de versnelling constant is. Maar in werkelijkheid verandert de versnelling wel degelijk. Om het verschil tussen de werkelijkheid en de benadering zo klein mogelijk te maken is het van belang dat de $\Delta t$ zo klein mogelijk is. Op deze manier verandert de versnelling gedurende $\Delta t$ zo min mogelijk.

Naast dit theoretische verschil zijn er ook afwijkingen in de versnellingsmeter die voor verschillen kunnen zorgen. In de R\&D opdracht onderzoek je welke invloed de verschillende soorten afwijkingen van de versnellingsmeter hebben op de plaatsbepaling.

## Vragen en opdrachten

17. Schets het $(v, t)$ - en $(s, t)$-diagram voor het geval dat:
a. de versnelling constant is en groter dan 0 ;
b. de versnelling lineair oploopt.
18. Vanuit stilstand meet de versnellingsmeter met een frequentie van 20 Hz de volgende 5 versnellingen achter elkaar in $\mathrm{m} / \mathrm{s}^{2}$ : 1,$1 ; 1,2 ; 1,1 ; 1,3 ; 1,4$. Wat is de afstand die de drone tijdens dit interval heeft afgelegd?
19. Verzin twee mogelijke toepassingen voor drones waar
a. een precieze plaatsbepaling niet van belang is;
b. een precieze plaatsbepaling erg belangrijk is.
20. Leg uit waarom nauwkeurige versnellingsmeters datapunten genereren met een hoge frequentie.

## R我D

## Opdracht: Coach

Doe de Coach opdracht bijbehorend bij deze paragraaf. Daarin ga je bekijken wat de precisie van je versnellingsmeter met je plaatsbepaling doet.

Maak en lever in:

R\&D 4a De antwoorden op de vragen van de Coach opdracht.
R\&D 4b De grafieken die je gemaakt hebt.

## Beloning:

Het goed uitvoeren van deze opdracht levert R\&D-punten op die gebruikt kunnen worden voor de sensoren.

## S\&B

Wil je meer leren, of hier later mee aan het werk, dan kun je de volgende opleidingen overwegen:

Aerospace engineering
Vliegtuigbouw
De nauwkeurigheid van sensoren is niet alleen bij vliegtuigen belangrijk, maar komt bij alle automatische systemen terug

## Leerdoelen

Na dit hoofdstuk kun je:

- benoemen welke sensoren een drone gebruikt voor plaats- en oriëntatiebepaling;
- bij een gegeven versnelling de snelheid bepalen;
- bij een gegeven snelheid de plaats bepalen;
- een model gebruiken voor de plaatsbepaling van een drone.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-33.jpg?height=895&width=621&top_left_y=178&top_left_x=132)


## De Vliegende Rechter

## Molenaars Kinderdijk strijden tegen drone-terreur

Molenaars in Kinderdijk worden horendol van de drones die om de haverklap opduiken rondom de molens waar zij wonen. "Met Pasen waren er wel zes op één dag. We worden continu bespied." Zij riepen deze week de hulp in van de gemeenteraad in de hoop dat die de toestellen verbiedt.

Maar dat is makkelijker gezegd dan gedaan, zegt burgemeester Dirk van der Borg van Molenwaard. "Er is op dit moment geen mogelijkheid om drones te verbieden. We hebben op alle mogelijke manieren gekeken hoe we hiertegen kunnen optreden."

Anja Noorlander is één van de Kinderdijkse molenaars: "We hebben er met zestien gezinnen intens veel last van. Het schaadt onze privacy in grote mate. Stel je voor dat je in je moestuin aan het werk bent en op vijf meter afstand hangt een drone die je langdurig filmt. Het is alsof er fotograferende mensen bij je over de schutting hangen, terwijl je niet weet wie het zijn."
AD 13-04-2018

## Wat denkt de Vliegende Rechter?

Ergens is het begrijpelijk dat er bij de molens op de Kinderdijk veel drones vliegen. Het is een mooi gebied en trekt ook toeristen...maar daar wonen ook mensen.

## VR4 Drone-terreur

Schrijf een vervolg op dit nieuwsbericht waarin een afspraak is gemaakt tussen een lid van de molenaarsfamilies, een dronefotograaf en een mediator.

- Zet beide standpunten zo helder en duidelijk mogelijk uiteen.
- De mediator doet haar best om ze te helpen. Geef drie afspraken die zij voorstelt om de twist op te lossen.


## 5 Externe krachten op een drone

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-34.jpg?height=315&width=595&top_left_y=408&top_left_x=134)

Figuur 5.1 De externe krachten op een vliegtuig
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-34.jpg?height=891&width=602&top_left_y=866&top_left_x=124)

Figuur 5.2 Een predator drone (boven) en een quadcopter (onder)
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-34.jpg?height=301&width=578&top_left_y=2085&top_left_x=134)

Figuur 5.3 De luchtstroom over een vleugel. Het pad dat de luchtstroom aan de bovenkant moet volgen is duidelijk langer dan het pad aan de onderkant.

De belangrijkste tegenwerkende krachten op een drone in de lucht zijn de luchtweerstand en de zwaartekracht. Deze krachten worden gecompenseerd door de voortstuwingskracht en de liftkracht. Wanneer een drone met vaste vleugels zich in een rechte lijn horizontaal met constante snelheid beweegt zijn deze krachten hetzelfde als bij het vliegtuig in figuur 5.1.

Normaal vliegt een vliegtuig niet precies evenwijdig met de grond maar onder een kleine hoek, de zogenaamde invalshoek $a$. Deze hoek is echter vrij klein, waardoor we voor de berekeningen in dit hoofdstuk kunnen aannemen dat de luchtweerstand gelijk is aan de voortstuwing en de liftkracht gelijk is aan de zwaartekracht.

Er bestaan niet alleen drones met vaste vleugels, maar ook drones met een rotor (zie figuur 5.2). Dit hoofdstuk behandelt de lift en de luchtweerstand voor deze twee typen drones. Aan de hand van deze informatie kun je bepalen wat de beste manier is om jouw drone te bouwen. Wil je er een die zo snel mogelijk van A naar B kan vliegen, of toch liever een drone die lang boven zijn doel kan blijven hangen?

### 5.1 De lift van een vleugel

De meeste vleugels en wieken zijn niet symmetrisch, maar hebben een ronde vorm (zie figuur 5.3), waardoor de lucht bovenaan de vleugel een langere weg moet afleggen dan onderaan de vleugel. Als de lucht over deze vleugels stroomt, beweegt deze aan de bovenkant sneller dan aan de onderkant. Dit verschil in snelheid zorgt voor een drukverschil, met een hogere luchtdruk onder de vleugel dan bovenaan de vleugel.

Dit drukverschil leidt ertoe dat de vleugel naar boven wordt getrokken. Je kunt de liftkracht $F_{l}$ berekenen met de volgende formule:

$$
F_{l}=\frac{1}{2} C_{l} \cdot \rho \cdot v^{2} \cdot A
$$

Hierin is:
$F_{l}$ de liftkracht (N)
$C_{l}$ de liftcoëfficiënt (geen eenheid)
$\rho$ de dichtheid van de lucht ( $\mathrm{kg} / \mathrm{m}^{3}$ )
$v$ de snelheid (m/s)
$A$ de vleugeloppervlakte $\left(\mathrm{m}^{2}\right)$

Wat je uit deze formule kunt zien is dat een vliegtuig of drone een voorwaartse snelheid moet hebben om voldoende liftkracht te genereren om in de lucht te blijven. De minimale snelheid die nodig is kun je uitrekenen door in de formule de maximale liftcoëfficiënt in te vullen en te kijken welke snelheid nodig is om een liftkracht te genereren die gelijk is aan de zwaartekracht.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-35.jpg?height=497&width=593&top_left_y=1005&top_left_x=109)

Figuur 5.4 De lift coëfficiënt als functie van de invalshoek
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-35.jpg?height=447&width=586&top_left_y=1664&top_left_x=118)

Figuur 5.5 Als de invalshoek toeneemt laat de luchtstroom aan de bovenkant van de vleugel los.

## Voorbeeld 2

Een drone met een massa van 10 kg vliegt net boven de grond met een snelheid van $20 \mathrm{~m} / \mathrm{s}$. De vleugeloppervlakte is $1,0 \mathrm{~m}^{2}$.
a Bereken welke liftcoëfficiënt deze drone moet hebben.
b Is de liftkracht groter of kleiner als de drone met dezelfde snelheid vliegt op een hoogte van 1 km ?
a Bereken eerst de zwaartekracht:
$F_{z}=m \cdot g=10 \times 9,81=98 \mathrm{~N}$, die is gelijk aan $F_{l}$
$C_{l}=\frac{2 \cdot F_{l}}{\rho \cdot v^{2} \cdot A}$
$C_{l}=\frac{2 \times 98}{1,293 \times 20^{2} \times 1,0}=0,38$
b De luchtdruk neemt af als je hoger gaat vliegen, dus $\rho$ wordt kleiner. Hierdoor zal de liftkracht afnemen.

## $C_{l}$ en overtrek

Je wilt bij voorkeur zo traag mogelijk kunnen vliegen, zodat je het minste last hebt van de luchtweerstand. Om dit te doen moet je zorgen dat de liftcoëfficiënt zo groot mogelijk is. De liftkracht hangt af van het snelheidsverschil waarmee de lucht over de vleugel stroomt. Dit verschil wordt groter als de vleugel een minder symmetrische vorm heeft of als je de hoek tussen je vleugel en de richting waarin je vliegt groter maakt. Als deze invalshoek a groter wordt, wordt de liftcoëfficiënt ook groter.

Zoals je in figuur 5.4 kunt zien, zit hier wel een maximum aan. Als je te schuin gaat vliegen zal de luchtstoom de vleugel namelijk niet meer kunnen volgen en loslaten van de vleugel. Dan ontstaat er turbulentie, waardoor de liftkracht afneemt. Dit verschijnsel heet overtrek. Een voorbeeld hiervan kun je zien in figuur 5.5.

Let op: Voor een aantal begrippen in de luchtvaart gebruik je ook in Nederland eigenlijk alleen de Engelse term:
overtrek $\longleftrightarrow$ stalling
invalshoek $\longleftrightarrow$ angle of attack

## Drones met een rotor

In plaats van vaste vleugels kan ook een rotor voor de liftkracht zorgen, zoals bij een helikopter. Een rotor bestaat eigenlijk uit twee of meer vleugels die in de rondte bewegen. Deze rotatie zorgt ervoor dat de lucht over de wieken (vleugels) van de rotor stroomt, zo genereert elke wiek een liftkracht. De bladen van een rotor zijn over het algemeen zo lang mogelijk, omdat de snelheid waarmee de wieken bewegen aan de uiteinden groter is dan aan de binnenkant van de rotor.

Het voordeel van het gebruik van een rotor is dat er geen minimumsnelheid is. Een helikopter kan stil in de lucht blijven hangen. Een helikopter kan ook alle kanten op vliegen, terwijl een vliegtuig min of meer zijn neus achterna moet vliegen. Dit leidt ertoe dat een drone met een rotor veel meer kan manoeuvreren dan een drone met vaste vleugels. Het nadeel van een rotor is dat deze meer energie verbruikt dan een drone met vaste vleugels. Daardoor kan een drone met een rotor minder lang in de lucht blijven en zal deze ook een lagere maximumsnelheid hebben.

### 5.2 Luchtweerstand

Als iets beweegt, werkt er altijd een kracht tegen: de luchtweerstandskracht. De luchtweerstandskracht is net als de liftkracht een gevolg van een drukverschil. Je berekent deze kracht dus op dezelfde manier als de liftkracht. Het verschil is dat $A$ nu niet de oppervlakte van de vleugels is, maar de frontale oppervlakte van de drone. De formule om de weerstandskracht te berekenen staat hieronder.

$$
F_{\mathrm{D}}=\frac{1}{2} C_{\mathrm{D}} \cdot \rho \cdot v^{2} \cdot A
$$

Hierin is:
$F_{\mathrm{D}}$ de weerstandskracht (N)
$C_{D}$ de weerstandscoëfficiënt (geen eenheid)
$\rho$ de dichtheid van de lucht ( $\mathrm{kg} / \mathrm{m}^{3}$ ),
$v$ de snelheid van de drone ( $\mathrm{m} / \mathrm{s}$ )
$A$ de frontale oppervlakte $\left(\mathrm{m}^{2}\right)$

De weerstandscoëfficiënt is bij een helikopter alleen afhankelijk van de vorm van de drone. Bij een vliegtuig hangt de weerstandscoëfficiënt ook af van de liftcoëfficiënt. Een grotere invalshoek $a$ leidt dus niet alleen tot een grotere liftcoëfficiënt, maar ook tot meer luchtweerstand.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-36.jpg?height=612&width=1075&top_left_y=1867&top_left_x=773)

Figuur 5.6 Het lift/weerstandsdiagram van een vliegtuig. De raaklijn vanuit de oorsprong geeft het punt aan waarbij de meeste lift wordt gegenereerd bij de minste weerstand.

## Voorbeeld 3

De drone waar figuur 5.6 bij hoort, heeft een massa van 100 kg , met vleugeloppervlakte van $4,0 \mathrm{~m}^{2}$ en de frontale oppervlakte is $1,0 \mathrm{~m}^{2}$. Bereken de weerstandskracht als de drone met een snelheid van $25 \mathrm{~m} / \mathrm{s}$ op zeeniveau vliegt.

Bereken eerst de zwaartekracht:
$F_{\mathrm{z}}=m \cdot g=100 \times 9,81=981 \mathrm{~N}$, die is gelijk aan $F_{l}$

$$
\begin{aligned}
& C_{l}=\frac{2 \cdot F_{l}}{\rho \cdot v^{2} \cdot A} \\
& C_{l}=\frac{2 \times 981}{1,293 \times 25^{2} \times 4,0}=0,61
\end{aligned}
$$

Zoek in de grafiek op welke $C_{\mathrm{D}}$ daarbij hoort $\rightarrow C_{\mathrm{D}}=0,036$.
Bereken dan de weerstandskracht:
$F_{\mathrm{D}}=\frac{1}{2} C_{\mathrm{D}} \cdot \rho \cdot v^{2} \cdot A=\frac{1}{2} \times 0,036 \times 1,293 \times 25^{2} \times 1,0=15 \mathrm{~N}$

### 5.3 Vermogen

Een drone verbruikt continu brandstof om in de lucht te blijven. Bij een vliegtuig moet de motor voldoende kracht genereren om de luchtweerstand te overwinnen, zodat het de juiste snelheid houdt. Bij een helikopter moet de rotor continu blijven draaien om voldoende liftkracht te genereren.

Het vermogen $P$ dat een vliegtuig nodig heeft om met een constante snelheid te kunnen vliegen kun je uitrekenen. Hiervoor moet je eerst de arbeid $W$ weten die de motor moet leveren om de luchtweerstand tegen te gaan:

$$
W=F_{\mathrm{D}} \cdot s
$$

Het vermogen kun je uitrekenen door de arbeid te delen door de tijd. Dit vermogen is dan:

$$
P=\frac{W}{t}=\frac{F_{\mathrm{D}} \cdot s}{t}=F_{\mathrm{D}} \cdot v
$$

Hierin is:
$P$ het vermogen (W)
$t$ de tijd in seconden (s)
$F_{\mathrm{D}}$ de luchtweerstandskracht (N)
$s$ de afgelegde afstand van de drone (m)
$v$ de snelheid van de drone ( $\mathrm{m} / \mathrm{s}$ )
Aangezien de luchtweerstand van een vliegtuig recht evenredig is met het kwadraat van de snelheid, is het benodigde vermogen recht evenredig met de derde macht van de snelheid. Dit betekent dat een toename van de snelheid tot een zeer grote toename van het benodigd vermogen zal leiden.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-38.jpg?height=529&width=598&top_left_y=478&top_left_x=135)

Figuur 5.7 De assen van een vliegtuig met de beweging daaromheen

Let op, ook hier geldt weer dat de Engelse termen vaker gebruikt worden dan de Nederlandse.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-38.jpg?height=189&width=324&top_left_y=1339&top_left_x=129)

Vliegtuigen die lang in de lucht moeten kunnen blijven worden daarom ook vaak ontworpen om met een zeer lage snelheid nog te kunnen blijven vliegen.

### 5.4 Besturing

De externe krachten in een vliegtuig hebben natuurlijk niet hetzelfde aangrijpingspunt. Dit betekent dat ook het moment in evenwicht moet zijn. Als dit niet het geval is gaat het vliegtuig draaien om een van de drie assen die hiernaast te zien zijn. Door het moment om een van de assen te manipuleren kan het vliegtuig worden bestuurd.

Op elke vleugel zitten 'ailerons'. Deze kunnen uitgeklapt worden om de liftkracht van een van beide vleugels te vergroten. Dit creëert een moment om de langs de as waardoor de drone gaat rollen. Dan wordt de liftkracht naar binnen gericht en zal de drone een scherpe bocht kan maken.

Op de kleinere vleugels in de staart zit het hoogteroer. Dit kan worden uitgeklapt of ingetrokken. Hierdoor verandert de lift die in de staart gegenereerd word en draait de drone om zijn dwarsas. Dit verandert de invalshoek en laat de drone naar boven of naar beneden vliegen.

Op het verticale deel van de staart zit het roer. Door het roer naar links of rechts uit te klappen gaat het verticale deel van de staart als een vleugel werken en creëert het een kracht naar links of naar rechts. Dit zorgt voor een moment om de verticale as, waardoor de drone een flauwe bocht zal maken

## Helikopters

De besturing van een helikopter werkt anders dan die van een vliegtuig. Een helikopter kan ook zonder te draaien naar links of naar rechts bewegen. Dit wordt gedaan door de rotor een klein beetje te draaien, waardoor de kracht niet alleen naar boven is gericht, maar ook naar de gewenste bewegingsrichting. Door de hele helikopter om een van zijn assen te draaien kan de kracht van de rotor sterker de gewenste kant op worden gericht.

## Vragen en opdrachten

## 21. Een bewegende drone

Een bewegende drone vliegt op een hoogte van $8,8 \mathrm{~km}$. De massa van de drone is 300 kg . De vleugels van de drone hebben een liftcoëfficiënt van 0,80 en een gezamenlijk oppervlak van is $5,0 \mathrm{~m}^{2}$.
a. Bereken de minimale snelheid die de drone moet hebben.
b. Zoek in figuur 5.6 de bijbehorende weerstandcoëfficiënt op en bereken de luchtweerstand die hierbij hoort.
c. Bereken het benodigde vermogen van de drone.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-39.jpg?height=829&width=529&top_left_y=1093&top_left_x=175)

Figuur 5.8 Besturing van de Tello Edu, Rob Lamping

## 22. Een helikopter

Steeds meer sportwedstrijden gebruiken helikopterdrones om met een camera boven het veld te vliegen en de wedstrijd te filmen.
a. Leg uit waarom een helikopter hier handiger is dan een vliegtuig.
b. Leg uit waarom het beter is meerdere lichte helikopters te nemen dan een zware.
c. Hoe belangrijk vind jij het dat deze drones helemaal veilig zijn?

## 23. De Predator

De Predator is een van de bekendste drones. Deze wordt al meer dan 15 jaar door het Amerikaanse leger gebruikt om verkenningsvluchten uit te voeren. Sinds een aantal jaren is er ook een bewapende variant van deze drone. Een eigenschap die de Predator zo geschikt maakt voor verkenningen is het feit dat hij erg lang in de lucht kan blijven.
a. Geef twee redenen waarom drones langer in de lucht kunnen blijven dan bemande vliegtuigen.
b. Leg uit waarom de vorm van de vleugels van de Predator (figuur 5.2) geschikt is voor een drone die lang in de lucht moet blijven.
c. Geef een voordeel dat bemande verkenningsvliegtuigen hebben ten opzichte van drones.

## 24. Overtrek

Als je drone te weinig liftkracht genereert kun je de liftcoëfficiënt vergroten door de stuurknuppel naar je toe te trekken. De neus van de drone gaat dan omhoog, waardoor de invalshoek groter wordt. Als de hoek te groot wordt, vindt er overtrek plaats. Wat overtrek zo gevaarlijk maakt is dat de liftcoëfficiënt niet meer vergroot en in sommige gevallen zelfs verkleint.
Leg met behulp van figuur 5.4 de bovenstaande bewering uit.

## 25. Besturen van een drone

Als je met een drone een bocht maakt, gebeurt er meer dan dat de drone om een as draait. Doordat de drone namelijk draait veranderen de krachten op de drone waardoor er nog veel meer dingen gebeuren.
a. Geef aan welke krachten veranderen wanneer de drone om zijn verticale as draait.
b. Welke beweging zal de drone dan maken?

## Praktische opdracht: Bouw een papieren vliegtuig

Dit klinkt alsof het een spelletje is voor kleine kinderen, maar door na te denken over de liftkracht en de luchtweerstand kun je een beter vliegtuigje bouwen dan je vroeger als kind deed.

Beantwoord de volgende vragen

- Wat zijn de belangrijkste eisen voor een papieren vliegtuig?
- Wat betekent dit voor de soort vleugels dat je nodig hebt?
- Hoe kun je de massa van het papier het beste verdelen?

Ontwerp twee papieren vliegtuigen, een die zo ver mogelijk moet vliegen en een die zo lang mogelijk in de lucht moet blijven. Test je ontwerp.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-40.jpg?height=90&width=295&top_left_y=292&top_left_x=429)
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-40.jpg?height=738&width=594&top_left_y=519&top_left_x=137)

Figuur 5.9 Een voorbeeld van een simulatie van een vleugelprofiel

## S\&B

Wil je meer leren, of hier later mee aan het werk, dan kun je de volgende opleidingen overwegen:

Aerospace engineering
Mechanical engineering

## Vliegtuigbouw

Hoewel er in Nederland geen complete vliegtuigen meer gebouwd worden, is het berekenen van de aerodynamische krachten ook belangrijk bij bijvoorbeeld het ontwerpen van auto's

## R我D <br> Opdracht: Maak je eigen vleugelprofiel.

De liftkracht is een van de belangrijkste dingen die je drone nodig heeft. Het kiezen van de juiste configuratie (vleugels of rotor, grote of kleine vleugels) beïnvloedt de prestaties van je uiteindelijke ontwerp in zeer sterke mate. Het is voor je bedrijf daarom belangrijk hier goed onderzoek naar te doen.

In de R\&D opdracht van dit hoofdstuk ga je kijken naar het profiel van je vleugel, of de wieken van je rotor. De liftcoëfficiënt is afhankelijk van de vorm. Voor deze opdracht gebruik je de simulator die je kunt vinden op: https://www.nasa.gov/stem-content/foilsim/

Deze simulator modelleert de profielen aan de hand van de zogenaamde NACA configuratie. Door in de simulator verschillende waarden in te vullen kun je verschillende profielen ontwerpen, die vervolgens in een simulatie getest worden om een lift en een weerstandscoëfficiënt te bepalen

Het doel is dat je een vleugelprofiel gaat ontwerpen voor je eigen drone. Denk hierbij goed na over de missie die jij wilt dat je drone gaat uitvoeren en wat voor vleugel (of wiek) profiel hier het beste bij past. Ontwerp in de simulator verschillende profielen om er een te vinden die bij jouw eisen past.

Maak en lever in:
R\&D 5a Een plaatje van het door jou ontworpen profiel.
R\&D 5b De bijbehorende lift- en weerstandscoëfficiënten.
R\&D 5c Een korte uitleg waarom voor jouw drone deze waarden goed zijn.

## Beloning:

Het goed uitvoeren van deze opdracht levert R\&D-punten op die gebruikt kunnen worden voor het ontwerp van de vleugels of rotor.

## Leerdoelen

Na dit hoofdstuk kun je:

- uitleggen welke krachten er op een drone werken;
- de liftkracht en de luchtweerstandskracht op een drone uitrekenen;
- beoordelen wat voor soort vleugels of rotor je nodig hebt voor een specifieke missie;
- uitrekenen hoe groot het vermogen is dat een drone verbruikt om met een gegeven snelheid in de lucht te blijven;
- uitleggen hoe een drone van bewegingsrichting verandert.


## De Vliegende Rechter

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-41.jpg?height=429&width=1023&top_left_y=331&top_left_x=765)

Figuur 5.10 De Boeing HorizonX

## Zware jongens

De Boeing HorizonX is een octocopter: een drone met acht propellers. Hij is bedoeld om grote ladingen te dragen en die over grote afstanden te vervoeren.
Zelf is het ook geen klein ding: het prototype weegt van zichzelf al 340 kilo en is 4,5 bij 5,5 meter. Het grootste gedeelte van dat gewicht zit ' $m$ in de flinke batterijen die de drone in het midden heeft zitten. Doordat de acht rotors van de motor aan de onder- en bovenkant andersom draaien kan de drone ook recht opstijgen.
Bron: Fair use DutchCowboys.nl

Ook bij vleugels en lift horen allerlei regels en ethische dilemma's. In dit hoofdstuk ga je kijken naar het formaat van de drones en de regels over de vlieghoogte die daarbij horen.

## Wat denkt de Vliegende Rechter?

## VR5

Bedenk hoe groot de drone die je met je groep gaat ontwerpen ongeveer zal worden.
Ga vervolgens op zoek naar de regels die aan een dergelijke drone verbonden zijn.

- Mag deze drone overal vliegen?
- Moet de bestuurder een brevet hebben of mag iedereen de drone besturen?

Tip: de site www.rijksoverheid.nl heeft een pagina met daarop de Nederlandse wetgeving met betrekking tot drones.

## Maak en lever in:

Een korte beschrijving (max 1 A4) met daarop de regels en wetten die van toepassing zijn op jouw drone.

Je gaat een lesuur lang aan de slag met twee (delen van) oude examenopgaven die aansluiten bij de stof van hoofdstuk 5 en/of met een klein experiment om de tilkracht van een drone te bepalen.

## I1 Cessna (natuurkunde examen vwo 2017 bewerkt)

Een Cessna is een eenmotorig vliegtuigje.
In tabel 1 staan gegevens van deze Cessna.

| Cessna |  |
| :--- | :--- |
| lengte | $7,3 \mathrm{~m}$ |
| spanwijdte | $10,7 \mathrm{~m}$ |
| hoogte | $3,0 \mathrm{~m}$ |
| tankinhoud | 19 L <br> $=55 \mathrm{~km} \mathrm{~h}^{-1}$ <br> $=55 \mathrm{~m} \mathrm{~s}^{-1}$ |
| kruissnelheid <br> (constant) | 678 km |
| max. vliegbereik | $100 \mathrm{pk} \mathrm{(hp)}$ |
| max. motorvermogen |  |

tabel 1
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-42.jpg?height=601&width=398&top_left_y=773&top_left_x=1374)

Figuur 1.1

Op een horizontaal rechtdoor vliegend vliegtuig werken drie krachten: de zwaartekracht $F_{\mathrm{z}}$, de motorkracht $F_{\mathrm{m}}$ en de kracht die de lucht op het vliegtuig uitoefent: $F_{\text {lucht }}$.
Deze $F_{\text {lucht }}$ hangt af van de stand van de vleugels.
$F_{\text {lucht }}$ kun je ontbinden in twee componenten. De component tegengesteld aan de vliegrichting is gelijk aan $F_{w, l u c h t}$. De component loodrecht op de vliegrichting heet liftkracht $F_{\text {lift }}$. $F_{\text {lucht }}$ maakt een hoek $a$ met $F_{\text {lift }}$. Zie figuur I. 1 hierboven. Deze figuur is niet op schaal.

Deze Cessna vliegt met zijn kruissnelheid op een constante hoogte. Het motorvermogen is dan $70 \%$ van het maximale motorvermogen. De beladen Cessna heeft op dat moment een massa van 710 kg .
a Bereken de grootte van hoek $a$ in deze situatie

De formule voor de liftkracht $F_{\text {lift }}$. is: $F_{\text {lift }}=\frac{1}{2} \rho A_{\text {vleugel }} C_{\text {lift }} v^{2}$ Hierin is:
$\rho \quad$ de dichtheid van lucht;
$A_{\text {vleugel }}$ de vleugeloppervlakte: de onderoppervlakte van beide voorvleugels samen;
$C_{\text {lift }}$ de liftcoëfficiënt;
$v \quad$ de snelheid ten opzichte van de lucht.
b Leid met behulp van deze formule de eenheid van Clift af.

In figuur I. 2 op de volgende bladzijde staan op schaal een zij-, boven- en vooraanzicht getekend van de Cessna.
c Bepaal met behulp van figuur 1.2 hieronder en tabel 1 de grootte van $C_{\text {lift }}$ voor de Cessna op kruissnelheid.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-43.jpg?height=2071&width=1626&top_left_y=369&top_left_x=249)

Figuur 1. 2

I2 Kruissnelheid (natuurkunde pilotexamen vwo 2012 bewerkt) Vliegtuigen en drones leggen een grote afstand van $A$ naar $B$ af met een zodanige snelheid, dat hun energieverbruik minimaal is: deze snelheid noemt men de kruissnelheid. Een te lage snelheid levert te weinig liftkracht op, een te hoge snelheid te veel wrijvingskracht. Naast het gewicht en het vleugeloppervlak blijkt ook de luchtdichtheid een factor die het energieverbruik en dus de kruissnelheid bepaalt.
In deze opgave over kruissnelheid kijk je uitsluitend naar horizontaal vliegen met constante snelheid.

Tijdens het vliegen van zowel vogels als vliegtuigen werken er twee verticale krachten: de liftkracht $F_{\mathrm{L}}$ en de zwaartekracht $F_{\mathrm{z}}$, en twee horizontale krachten: de motor- of spierkracht $F_{\mathrm{m}}$ en de wrijvingskracht $F_{\mathrm{w}}=k v^{2}$.
De verhouding $f=\frac{F_{\mathrm{L}}}{F_{\mathrm{w}}}$ is karakteristiek voor de manier van vliegen en bepaalt mede het energieverbruik.

Voor een vliegtuigje (de Cessna) geldt: $m=620 \mathrm{~kg}$ enk $=0,44 \mathrm{~kg} / \mathrm{m}$ Bij de kruissnelheid van de Cessna geldt tevens: f=7,0 a Bereken de kruissnelheid van de Cessna.

Op kruissnelheid levert de Cessna een mechanisch vermogen van $3,8 \cdot 10^{4} \mathrm{~W}$.
De benzinemotor heeft een rendement van $24 \%$. Op een bepaald moment heeft de Cessna 75 L benzine in de tank.
b Bereken hoe lang de Cessna hiermee kan vliegen op kruissnelheid.
Vliegtuigen en drones zijn in staat de waarde van $f$ iets aan te passen.
c Beredeneer aan de hand van de definitie of de waarde van $f$ bij kruissnelheid minimaal of maximaal is.

## Experiment Tilkracht bepalen

## Benodigdheden

- drone
- krachtmeter/veerunster
- dun stevig touw (vislijn)
- grote, hoge ruimte


## Aanpak

1 Verbind de krachtmeter met het touw aan de drone.
2 Houd de krachtmeter stevig vast.
3 Laat de drone langzaam en voorzichtig stijgen.

| $f(\mathrm{rpm})$ | $F_{\text {til }}(\mathrm{N})$ |
| :--- | :--- |
|  |  |
|  |  |
|  |  |

4 Zorg dat de drone op een stabiele hoogte blijft.
5 Meet het toerental (bedenk zelf hoe) en meet de tilkracht $F_{\text {til }}$ (met de krachtmeter).
6 Herhaal de vorige opdrachten bij een hoger toerental. Maak een tabel zoals hiernaast. Doe metingen bij minstens 6 verschillende waarden van het toerental.

7 (optioneel) Bereken de massa die de drone kan vervoeren.

## 6 Vervorming, interne krachten, materialen

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-45.jpg?height=395&width=515&top_left_y=485&top_left_x=191)

Figuur 6.1 Een oude stenen brug met bogen.

Behalve externe krachten, spelen ook interne krachten een rol in drones. Deze krachten werken binnenin de materialen, die kapot gaan als ze niet tegen deze krachten bestand zijn.
Ook in andere constructies zijn interne krachten belangrijk, bijvoorbeeld bij bruggen. Want waarom hebben oudere stenen bruggen zo vaak een boogvorm?

In dit hoofdstuk kijk je naar interne krachten die een rol spelen in constructies als bruggen en drones. Hierbij zijn de volgende begrippen belangrijk:

- vervorming
- (relatieve) rek
- elasticiteitsmodulus
- treksterkte en druksterkte
- vorm van een constructie
- verschillen tussen materialen


### 6.1 Vervorming

De meeste materialen vervormen als je er een kracht op uitoefent. Bij elastische vervorming komt het materiaal weer terug in zijn oorspronkelijke vorm, als je er geen kracht meer op uitoefent. Als je bijvoorbeeld een veer niet te ver uitrekt, is de uitrekking $u$ recht evenredig met de kracht $F_{\text {trek }}$ die je er op uitoefent ( $F=C \cdot u$, met $C$ is de veerconstante). Bij een bepaalde grootte van de uitgeoefende kracht ( $F_{\text {trek_max }}$ ) krijg je echter blijvende of plastische vervorming. De veer komt niet meer terug in zijn oude vorm.

Als je op een draad een kracht uitoefent, blijkt de uitrekking $\Delta l$ recht evenredig met de oorspronkelijke lengte $l_{0}$ van de draad. De verhouding tussen de uitrekking $\Delta l$ en de oorspronkelijke lengte $l_{0}$ noem je de (relatieve) rek $\varepsilon$ :

$$
\varepsilon=\frac{\Delta l}{l_{0}}
$$

De uitrekking en de oorspronkelijke lengte hebben dezelfde eenheid, dus heeft $\varepsilon$ geen eenheid.
Bijvoorbeeld bij een elastiekje dat je uitrekt tot het twee maal zo lang is, is de rek $100 \%$, ofwel $\varepsilon=\frac{\Delta l}{l_{0}}=1$.

Als je op een draad een trekkracht uitoefent, rekt een dikke draad minder uit dan een dunne draad van hetzelfde materiaal. Het blijkt dat de kracht, bij een bepaalde rek, kwadratisch evenredig is met dikte van de draad. Je kunt daarom beter kijken naar de kracht per eenheid van oppervlakte.

Dat is de mechanische spanning of kortweg spanning $\sigma$ (in $\mathrm{Pa}=$ $\mathrm{N} / \mathrm{m}^{2}$ ):

$$
\sigma=\frac{F}{A}
$$

met $F$ is de kracht (in $N$ ) en $A$ is de oppervlakte van de dwarsdoorsnede (in $\mathrm{m}^{2}$ ).

Bij veel materialen is de rek $\varepsilon$ recht evenredig met de spanning $\sigma$, mits de vervorming elastisch is. De elasticiteitsmodulus $E$ geeft aan hoeveel spanning je op een material moet zetten om het een rek (in theorie) van $100 \%$ te geven. De elasticiteitsmodulus van materialen kun je vergelijken met de veerconstante.
Waar de veerconstante de kracht per meter uitrekking is, is de elasticiteitsmodulus de spanning per $100 \%$ uitrekking.
De formule voor $E$ is:

$$
E=\frac{\sigma}{\varepsilon}
$$

met als eenheid voor $E$ ook $\mathrm{Pa}\left(=\mathrm{N} / \mathrm{m}^{2}\right)$.
De meeste stoffen hebben een elasticiteitsmodulus in de orde van $10^{8}$ à $10^{11} \mathrm{~Pa}$ (zie Binas tabel $8 \mathrm{t} / \mathrm{m} 10$ en tabel 6.1 ).

In figuur 6.2 zie een spanning, rek-diagram. Het eerste deel van de grafiek is recht. Hier is sprake van elastische vervorming: de spanning is recht evenredig met de rek. Hierbij is de steilheid van de grafiek $(=\sigma / \varepsilon)$ gelijk aan de elasticiteitsmodulus $E$.

Vanaf een grenswaarde is de vervorming niet meer elastisch, maar plastisch. Er is dan nauwelijks extra kracht nodig om het materiaal nog meer uit te rekken. Dit wordt ook wel vloeiing genoemd.
Na het vloeien kun je op het materiaal nog meer kracht uitoefenen tot de treksterkte, dat is de spanning $\sigma_{\text {trek }}$, waarbij het materiaal net niet breekt.
De treksterkte $\sigma_{\text {trek }}$ is een stofeigenschap die je vindt in Binas tabel 8 en 10B, en in tabel 6.2 hieronder. Daar gaat $\$ 6.2$ verder op in.

| naam | elasticiteitsmodulus <br> $E\left(10^{9} \mathrm{~Pa}\right)$ | treksterkte <br> $\sigma_{\text {trek }}\left(10^{6} \mathrm{~Pa}\right)$ |
| :--- | :--- | :--- |
| aluminium | 71 | 310 |
| carbonfiber | 146 | 2400 |
| hard pvc | $2-4$ | $50-60$ |
| hout | $10-20$ | $80-160$ |
| nylon | $2-4$ | 80 |
| staal | 200 | 500 |

Tabel 6.1
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-47.jpg?height=872&width=486&top_left_y=1254&top_left_x=157)

Figuur 6.3 Materiaaltest met een trekbank

### 6.2 Interne krachten

Als er een resulterende kracht werkt op een voorwerp zal de snelheid ervan veranderen ( $2^{\mathrm{e}}$ wet van Newton). Als de snelheid van een voorwerp niet verandert, betekent dat echter niet dat er geen krachten op werken. Wat het wel betekent, is dat al die krachten bij elkaar samen geen resulterende kracht opleveren ( $1^{\mathrm{e}}$ wet van Newton). Ga maar na: als je een boog hebt gespannen zal die boog, zolang je hem vasthoudt, geen verandering van snelheid doormaken. De boog bewoog niet en hij zal niet gaan bewegen. Er werken uiteraard wel allerlei krachten: je spierkracht bijvoorbeeld, maar ook de spankracht.

De spankracht is een typisch voorbeeld van een interne kracht: een kracht die binnen in een voorwerp werkt, vaak (maar niet altijd) veroorzaakt door een kracht die door een ander voorwerp wordt uitgeoefend. In dit voorbeeld is de spankracht een reactie op de spierkracht.

Als je een gitaar op tafel legt, werken daar de zwaartekracht van de aarde en de normaalkracht van de tafel op. Deze twee krachten heffen elkaar precies op, zodat de resulterende kracht nul is en de gitaar niet beweegt. Dit zijn echter niet alle krachten: de snaren zijn gespannen, dus is er sprake van spankracht.
Deze interne krachten zullen je gitaar echter nooit kunnen laten bewegen: voor de snelheidsverandering van een voorwerp is een externe kracht nodig. Alle interne krachten van de gitaar bij elkaar kunnen namelijk niet leiden tot een resulterende kracht. Ga maar na: de snaar trekt altijd net zo hard aan de hals, als de hals aan de snaar. Dit geldt voor elke interne kracht.

Wat wel kan gebeuren, is dat een snaar knapt. Wanneer een snaar knapt, hangt onder andere af van de treksterkte ( $\sigma_{\text {trek }}$ ) van het materiaal waarvan de snaar is gemaakt. De treksterkte van nylon is vele malen groter dan die van bijvoorbeeld katoen.

De formule voor de treksterkte is analoog aan die voor spanning:
$\sigma_{\text {trek }}=\frac{F_{\text {trek_max }}}{A}$
Hierin is:

- $\quad F_{\text {trek_max }}$ de maximale trekkracht van een voorwerp (N),
- $\sigma_{\text {trek }}$ de treksterkte van het materiaal (Pa of $\mathrm{N} / \mathrm{m}^{2}$ ), tabel 6.1
- $A$ de oppervlakte van de (dwars)doorsnede $\left(\mathrm{m}^{2}\right)$.

Natuurlijk kun je niet alleen aan een materiaal trekken, je kunt er ook op drukken. Op precies dezelfde manier als hierboven voor de treksterkte beschreven, werkt ook de druksterkte ( $\sigma_{\text {druk }}$ ) van een materiaal. Als de maximale drukkracht van een voorwerp wordt overschreden, zal het voorwerp breken, scheuren of onherstelbaar vervormen. Voor de drukkracht geldt hetzelfde als voor de trekkracht: hoe 'dunner' het voorwerp, hoe sneller het zal vervormen of breken.

### 6.3 Materialen

Bij het ontwerp van drones is het natuurlijk van belang dat je rekening houdt met trek- en druksterkte van de materialen waaruit de drone bestaat. Daarnaast is dichtheid een belangrijke eigenschap, een drone moet immers niet te zwaar worden. Zo heeft beton een grote druksterkte, maar het is uiterst ongeschikt is om een drone van te maken. Je moet dus compromissen sluiten tussen zaken als sterkte, massa en natuurlijk de prijs van het materiaal.

| Naam | Trek- <br> druksterkte <br> $(\mathrm{MPa})$ | Dichtheid <br> $\left(\mathrm{kg} / \mathrm{m}^{3}\right)$ | Relatieve <br> prijsindicatie |
| :--- | :--- | :--- | :--- |
| nvlon 66 | 80 | 1140 | $€ €$ |
| HDPE | 32 | 970 | $€$ |
| ABS | 39 | 1060 | $€ €$ |
| koolstof- <br> vezels | 3500 | 1300 | $€ € € € €$ |

Tabel 6.2 Enkele materialen voor droneonderdelen en hun eigenschappen

Veel onderdelen van goedkopere drones worden doorgaans gemaakt van kunststoffen als nylon. Nylon heeft een treksterkte van ongeveer 80 MPa , de druksterkte is ongeveer even groot. Voor duurdere drones gebruikt men ook wel koolstofvezel, dat veel sterker is en niet eens zo veel zwaarder. Het is echter wel veel duurder.

Vier materialen die men vaak gebruikt voor onderdelen van drones zijn nylon 66, HDPE (high density polyethylene), Acrylonitril-butadiëen-styreen (ABS) en koolstofvezels. In tabel 6.2 staat een overzicht van enkele belangrijke eigenschappen van deze materialen.

In de R\&D-opdracht aan het einde van dit hoofdstuk ga je bouwen met spaghetti, een licht, redelijk sterk materiaal. In practicum 1 ga je van spaghetti de elasticiteitsmodulus $E$ en de treksterkte $\sigma_{\text {trek }}$ bepalen.

- Overleg met je docent hoe en wanneer je practicum 1 (of een alternatief daarvan) uitvoert.

Voor je aan het practicum begint nog een stukje theorie:
Je kunt een staaf of een balk met een (vrije) lente $L$ op verschillende manieren belasten met een kracht $F$ dwars of de balk of staaf. Het voorwerp zal dan doorbuigen. De doorbuiging $d$ is dan omgekeerd evenredig met elasticiteitsmodulus $E$, zoals weergegeven in de onderstaande figuur.

| belastingsituatie |  | doorbuiging |
| :--- | :--- | :--- | :--- |
| Vrij opgelegd op twee <br> steunpunten met een <br> belasting in het midden |  |  |

Figuur 6.4 Twee verschillende manieren om een staaf te belasten

De grootheid $I_{0}$ (het traagheidsmoment) heeft te maken met de vorm van de staaf of balk. In de bouwkunde, de civiele techniek en de vliegtuigbouw zoekt men dan ook staven of balken met een zo hoog mogelijk traagheidsmoment in de draagrichting met een laag materiaalverbruik. Zo'n staaf of balk heeft een grote draaglast bij een kleine doorbuiging.

Voor een staaf (zoals spaghetti) met een cirkelvormige dwarsdoorsnede met straal $r$ geldt: $I_{\mathrm{O}}=\frac{\pi r^{4}}{4}$.

## Vragen en opdrachten

26. Waarom wordt in de bouw vaak gewapend beton (beton met staaldraden erin) gebruikt? Onderbouw je antwoord met gegevens van het internet (denk aan trek- en druksterkte).
27. Hieronder zie je een oude tekening met een ontwerpconcept voor een brug in New York. Geef in de tekening aan welke delen van de brug vooral druk- en welke vooral trekkrachten ondervinden.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-49.jpg?height=319&width=1058&top_left_y=1137&top_left_x=810)

Figuur 6.5 Brugontwerp in New York.

## 28. Gitaarsnaar

In dit hoofdstuk komen twee belangrijke materiaaleigenschappen aan de orde: de treksterkte en de elasticiteitsmodulus.
a Als je een gitaarsnaar spant om de toon lager te maken, kost dat veel kracht.
Leg uit met welk van de twee eigenschappen dat te maken heeft.
b Als je de gitaarsnaar te strak spant, kan hij knappen.
Leg uit met welk van de twee eigenschappen dat te maken heeft.

## 29. Koolstofvezels

a. Hoe komt het dat koolstofvezels zoveel sterker zijn dan de andere materialen? Gebruik voor je antwoord het internet.
b. Koolstofvezels zijn het zwaarste materiaal in tabel 6.2. Wat zorgt er dan voor dat een drone van koolstofvezels uiteindelijk toch lichter is?

## 30. Staaldraad

Aan een staaldraad van 23 m lang hangt een voorwerp van 15 kg . De staaldraad heeft een diameter van $1,2 \mathrm{~mm}$ en rekt 15 mm uit.
a. Bereken de (relatieve) rek.
b. Bereken de mechanische spanning.
c. Bereken de elasticiteitsmodulus van de staaldraad.
d. Leg met behulp van Binas uit of je antwoord op c kan kloppen.
e. bereken hoeveel kg je aan de draad kunt hangen voor hij knapt.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-50.jpg?height=532&width=589&top_left_y=248&top_left_x=117)
31. Elastiek (havo-pilotexamen 2012 bewerkt)

Jaap doet een aantal proeven met een elastiek dat postbodes vaak gebruiken. Allereerst bepaalt hij de veerconstante $C$ van het elastiek. Hij knipt het elastiek door en trekt eraan met een krachtmeter. Hij meet de lengte $\ell$ van het elastiek als functie van de kracht $F$. Zijn metingen heeft hij in een grafiek weergegeven, zie figuur 6.6.
a Bepaal de veerconstante $C$ van dit elastiek.

Voor de veerconstante $C$ van een elastiek dat niet al te ver uitrekt, geldt: $C=\frac{E \cdot A}{\ell_{0}}$
Met:

- E is de elasticiteitsmodulus (in Pa)
- A is de oppervlakte van de dwarsdoorsnede (in m²)
- $\ell_{0}$ is de lengte van het onbelaste elastiek (in m)
b Leg uit waarom het elastiek niet te ver uitgerekt mag worden voor de geldigheid van deze formule.
c Toon met behulp van bovenstaande formule aan dat de eenheid van de elasticiteitsmodulus $E$ gelijk is aan Pa.
d Leid de formule af uit formules in dit hoofdstuk

De doorsnede van het onbelaste elastiek is een rechthoek met afmetingen $1,0 \mathrm{~mm} \times 7,5 \mathrm{~mm}$.
e Zou het-elastiek dat Jaap gebruikt van rubber gemaakt kunnen zijn? Licht je antwoord toe met een berekening.

## R <br> ![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-50.jpg?height=98&width=295&top_left_y=1596&top_left_x=418)

## S\&B

Wil je meer leren, of hier later mee aan het werk, dan kun je de volgende opleidingen overwegen:

## Material sciences

Mechanical engineering
Ook hier is het berekenen van krachten binnen een materiaal voor alle technische velden belangrijk.

## R\&D: brugbouwwedstrijd

Maak en lever in:

R\&D 6 Bouw met ongekookte spaghettistokjes en een lijmpistool een brug met een overspanning (= de afstand die de brug overbrugt) van minstens 30 cm . Het doel is om zo hoog mogelijke verhouding (draagvermogen/eigengewicht) te halen. Het draagvermogen test je door de brug steeds meer te belasten, totdat hij instort. Maak slim gebruik van de trek- en druksterkte van spaghetti!

## Beloning:

Het goed uitvoeren van deze opdracht levert R\&D-punten op die gebruikt kunnen worden voor het ontwerp van de romp.

## Leerdoelen

Na dit hoofdstuk kun je:

- uitleggen wat relatieve rek en mechanische spanning is;
- redeneren en rekenen met spanning, rek en elasticiteitsmodulus
- uitleggen wat interne krachten zijn en voorbeelden noemen;
- treksterkte van een materiaal berekenen.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-51.jpg?height=227&width=413&top_left_y=178&top_left_x=299)


## De Vliegende Rechter

## Is een drone beschieten boven eigen terrein een onrechtmatige daad?

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-51.jpg?height=409&width=598&top_left_y=515&top_left_x=158)

Figuur 6.7 Jager met buks
Mag je met je luchtbuks op een drone schieten als die hinderlijk boven je achtertuin hangt? Die vraag lag onlangs voor bij een rechtbank in Gelderland. Een complex vraagstuk, waarbij niet alleen het eigendomsrecht, maar ook de privacywetgeving om de hoek komt kijken.

## Burenruzie

Aanleiding voor de rechtszaak is een uit de hand gelopen burenruzie. Een man had met zijn drone boven de tuin van de buren gehangen. Toen de dronepiloot na afloop de beelden bekeek, zag hij dat een buurjongen met een buks op het toestel had geschoten, met - volgens de bezitter van de drone - enige beschadigingen tot gevolg. De man spande daarop een zaak aan tegen de buren, maar die beweerden vervolgens in hun privacy te zijn aangetast door de drone, en eisten op hun beurt een schadevergoeding.

Een lastige casus: in de regelgeving voor het vliegen met drones wordt immers niet gesproken over een verbod op het vliegen boven iemands privéterrein. En op het gebied van privacybescherming zijn er geen specifieke bepalingen voor drones opgenomen in de wetgeving, hoewel het Europees Verdrag tot bescherming van de rechten van de mens (EVRM) volgens de rechter voldoende handvatten biedt: de aanwezigheid van de drone, of die nu opnamen maakt of niet, "zorgt voor een gevoel van onvrijheid waarvan men in de eigen woning gevrijwaard behoort te blijven." Maar dat is nog geen aanleiding om dan maar voor eigen rechter te gaan spelen.
Bron: Drone watch 18 mei 2017

## Wat denkt de Vliegende Rechter?

## VR6

https://www.eudronebewijs.n//blogs/actueel/privacy-en-drones
Deze site geeft aan wat een drone-operator wel of niet mag doen om de privacy van burgers te respecteren.
a. De luchtbuks-gebruikende buurman vraagt jou om een verdediging voor hem voor te bereiden. Schrijf een verdediging (max 1 A4) op basis van schending van privacy. Gebruik daarbij vijf punten uit het rapport die zijn standpunt ondersteunen.
b. Geef aan welke van deze punten impact hebben op het ontwerp van een drone. Wat zou de drone ontwerper moeten doen om de rijksoverheid tegemoet te komen?

## 7 Aandrijving

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-52.jpg?height=378&width=579&top_left_y=813&top_left_x=156)

Figuur 7.1 Eenmalige voortstuwing bij een zweefvliegtuig d.m.v. een lier.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-52.jpg?height=320&width=569&top_left_y=1439&top_left_x=158)

Figuur 7.2 Permanente voortstuwing bij een zweefvliegtuig met een uitklapbare hulpmotor.

De aandrijving is het systeem dat ervoor zorgt dat de drone zich voortbeweegt. Het centrale deel van de aandrijving is de motor. Hier hoort ook nog de energievoorziening bij.

### 7.1 Voortstuwing

## Inleiding

Voortstuwing komt neer op de effectieve kracht die het aandrijvingssysteem levert waardoor de drone zich voortbeweegt, ofwel de stuwkracht.
Bij de voortbeweging van een zweefvliegtuig in de lucht kun je gebruik maken van wat de natuur biedt: zwaartekracht en luchtstromingen. Wel moet je het zweefvliegtuig eerst met voldoende startsnelheid de lucht in brengen. Hiervoor gebruikt je eenmalige voortstuwing, bijvoorbeeld met behulp van een lier (startsnelheid $100 \mathrm{~km} / \mathrm{h}$ tot 450 m hoogte, zie figuur 7.1).
Zonder verdere voortstuwing daalt het zweefvliegtuig in de lucht omdat het onderhevig is aan luchtwrijving en de zwaartekracht. Door echter onder een bepaalde glijhoek te dalen behoud je voldoende snelheid en lift en kun je een relatief grote afstand afleggen. Een modern zweefvliegtuig legt vanaf 500 meter hoogte wel 20 kilometer af.
Door gebruik te maken van een thermiekbel (opstijgende warme lucht) win je weer hoogte en blijf je langer in de lucht. Thermiek ontstaat doordat de zon het aardoppervlak opwarmt die op haar beurt de bovenliggende lucht verwarmt. Zweefvliegtuigen vliegen zo uren op zonne-energie!
In heuvelachtige gebieden treden ook opwaartse luchtstromingen (hellingwinden) op waarvan zweefvliegers gebruik maken.
Met het plaatsen van een motor op een zweefvliegtuig lever je permanente voortstuwing (zie figuur 7.2) tegengesteld gericht aan de luchtwrijving waardoor je langer op constante hoogte kan vliegen. De uitklapbare motor is vooral bedoeld voor momenten dat de vlieger hoogte wil winnen, maar zich niet in een thermiekbel bevindt.

In deze paragraaf kijk je naar het voortstuwingsprincipe, twee methodes van voortstuwing en twee verschillende motoren die je hierbij kunt gebruiken en waarmee je een drone kunt uitrusten.

- straalaandrijving
- propelleraandrijving
- brandstofmotor
- elektromotor

Verder gaat het over de grootheid impuls. Met behulp van impulsberekeningen ga je de stuwkracht berekenen.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-53.jpg?height=384&width=372&top_left_y=616&top_left_x=177)

Figuur 7.3 Straalaandrijving vs propelleraandrijving
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-53.jpg?height=292&width=554&top_left_y=1921&top_left_x=177)

Figuur 7.4 Derde wet van Newton actiekracht = - reactiekracht

## Voortstuwing

Voor de voortstuwing van je drone heb je een krachtbron nodig: de motor. Het principe van voortstuwing bij vliegtuigen is het naar achteren versnellen van een hoeveelheid gas. Volgens de derde wet van Newton ontstaat er een tegengestelde kracht op de drone, de stuwkracht. De stuwkracht kan op twee manieren geleverd worden.

Bij straalaandrijving krijgt een kleine massa gas na verbranding een hoge versnelling, de drone bereikt daardoor hoge snelheden. Het nadeel is echter dat de luchtweerstand hierbij hoog is en daarmee ook het brandstofverbruik.

Bij propelleraandrijving krijgt een grote massa lucht een lage versnelling, de drone bereikt daardoor minder hoge snelheden. Het nadeel van de propeller is dat zijn omvang ook bijdraagt aan de luchtweerstand. Echter vanwege de minder hoge snelheid zal de totale luchtweerstand veel lager zijn vergeleken met straalaandrijving. Het brandstofverbruik ligt dan ook aanzienlijk lager, wat propelleraandrijving geschikt maakt voor drones die minder snel vliegen maar wel lang in de lucht verblijven.

Als krachtbron voor de stuwkracht onderscheid je twee motortypen:
In een brandstofmotor (verbrandingsmotor) vindt verbranding van een brandstof plaats waarbij de vrijgekomen energie omgezet wordt in bewegingsenergie. Omdat de brandstofmotor naast bewegingsenergie veel onbruikbare warmte produceert ligt het rendement van de brandstofmotor beneden de $42 \%$.

De elektromotor zet elektrische energie om in bewegingsenergie. De energiebron hiervoor is de batterij, maar kan ook een brandstof zijn die een brandstofcel verbruikt. Het voordeel van de elektromotor is het hoge rendement (circa 95\%) vanwege de minimale warmteproductie bij de energieomzettingen.

## Impuls

Gooi een bal naar voren als je met schaatsen op het ijs staat: de bal duwt je achteruit (figuur 7.4). Laat een opgeblazen ballon los en het is de uitstromende lucht die de ballon in tegengestelde richting verplaatst. Met deze experimenten toon je aan dat er een reactiekracht (stuwkracht) is die het object voortduwt.

Steeds gaat het om krachten die er voor zorgen dat een voorwerp een ‘hoeveelheid beweging’ krijgt. Dat heet in de natuurkunde impuls $p$ :

$$
\vec{p}=m \cdot \vec{v}
$$

Hierin is:
$\vec{p}$ de vectoriele grootheid impuls ( $\mathrm{kg} \mathrm{m} \mathrm{s}^{-1}$ )
$m$ de massa die het object met snelheid $v$ heeft (kg)
$\vec{v}$ de vectoriele grootheid snelheid van de massa $\left(\mathrm{m} \mathrm{s}^{-1}\right)$.

Voor een object met massa $\boldsymbol{m}$ die een snelheidsverandering $\Delta \boldsymbol{v}$ ondergaat, geldt de impulsverandering $\Delta p$ :

$$
\Delta p=m \cdot \Delta v
$$

Als een kracht op een object werkt dan verandert de impuls van het object in de tijd. Voor een object waar een constante kracht $F(=m \cdot a$ volgens de tweede wet van Newton) gedurende een bepaalde tijdsduur $\Delta t$ op werkt geldt:

$$
F \cdot \Delta t=m \cdot a \cdot \Delta t=m \cdot \Delta v=\Delta p
$$

### 7.2 Energievoorziening

In het voorbeeld van de opgeblazen 'vliegende' ballon blijkt dat de ballon niet lang in de lucht blijft. De opgeslagen energie (potentiële energie in de vorm van luchtdruk en spanning in het ballonmateriaal veroorzaakt door uitrekking van het ballonmateriaal) is hier beperkt en voor korte tijd aanwezig. Voor een langere verblijftijd in de lucht moet je meer energie in een kleinere ruimte met zo min mogelijk massa opslaan. Je drukt dit uit in energiedichtheid ( $\mathrm{Jkg}^{-1}$ ). Ook bij het ontwerp van je drone is dit een uitgangspunt.

In deze paragraaf kijk je naar de energievoorziening die nodig is om de drone in beweging te krijgen en in de lucht te houden. Het gaat dan over de volgende drie energiebronnen:

- brandstof
- batterijen
- zonne-energie en zonnecellen


## Brandstof

Chemische energie is de energie die opgeslagen zit in de bindingen tussen de verschillende atomen van een molecuul. Je kunt je dan ook voorstellen dat elk molecuul en daarbij elke stof een andere chemische energiewaarde heeft. Tabellen 28B, 56 en 57 van Binas geven waarden van de chemische energie van stoffen.

Een verbranding is een exotherme reactie. Bij een exotherme reactie komt de chemische energie vrij in de vorm van onder andere warmte. Na de exotherme reactie bevatten de eindstoffen minder chemische energie dan de beginstoffen. Hierbij geldt de wet van energiebehoud:
$E_{\text {beginstoffen }}=E_{\text {eindstoffen }}+E_{\text {vrijgekomen }}$
De reactie-energie, $\Delta E_{\text {reactie }}$ is afgesproken als:
$\Delta E_{\text {reactie }}=E_{\text {eindstoffen }}-E_{\text {beginstoffen }}$
Uit de twee bovenstaande formules volgt:
$\Delta E_{\text {reactie }}=-E_{\text {vrijgekomen }}$
Een groot nadeel bij het gebruik van brandstof als energiebron in een brandstofmotor is het lage rendement vanwege het warmteverlies.

## Batterijen

Als een drone is uitgerust met een elektromotor dan is de energievoorziening hiervoor de batterij. Ook in de batterij is de energie opgeslagen in de vorm van chemische energie. De meest gebruikte batterij bij drones is de Lithium-ion Polymeer batterij.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-55.jpg?height=518&width=572&top_left_y=212&top_left_x=154)

Figuur 7.5 Daniell cel

| Brandstof | Stookwaarde <br> $10^{9} \mathrm{~J} \mathrm{~m}^{-3}$ | Dichtheid <br> $\mathrm{kg} \mathrm{m}^{-3}$ |
| :--- | :---: | :---: |
| Biodiesel | 33 | 880 |

Tabel 7.1 Gegevens biodiesel

Het principe van elke batterij kun je beschrijven aan de hand van de Daniell cel (Figuur 7.5). Dit is een elektrochemische cel, waarbij aan de negatieve elektrode (anode) een redox-halfreactie plaatsvindt en aan de positieve elektrode (kathode) de andere redox-halfreactie.

## - In practicum 2 bouw je zelf een batterij.

Het nadeel van de batterij is de relatief lage energiedichtheid. De Lithium-ion Polymeer (Lipo) batterij heeft in vergelijking met andere batterijen een hogere energiedichtheid ( $0,9 \mathrm{MJ} \mathrm{kg}^{-1}$ ). Toch is dat nog een factor 40 lager dan bij fossiele brandstoffen en een factor 130 lager dan bij waterstof. Het voordeel van de batterij is dat er geen extra massa voor opslag bijkomt, zoals de zware tanks waarin brandstof opgeslagen zit.

## Vragen en opdrachten

32. "What goes up, must come down"
a. Beredeneer vanuit het oogpunt van de thermiekbel waarom een zweefvliegtuig niet oneindig hoog kan opstijgen (2 redenen).
b. Bespreek je antwoord in een groep van 4 leerlingen.
c. Kwam je antwoord overeen met de overige leerlingen? Wat was anders? Wat had je goed? Wat moest je aanpassen?

## 33. Stuwkracht

Een propellermotor van een 2 -motorig vliegtuig verplaatst netto $15 \mathrm{~m}^{3}$ lucht per seconde ( $\rho_{\text {lucht }}=1,0 \mathrm{~kg} \mathrm{~m}^{-3} ; A_{\text {motor_uit }}=1,0 \mathrm{~m}^{2}$ ). Bereken de stuwkracht die het vliegtuig ondervindt.

- Hierna overleg je met de docent of je nu practicum 3 uitvoert.


## 34. Brandstof

De waterraket uit practicum 2 moet je ombouwen en voorzien van een raketmotor en chemische energie.
a. Geef de reactievergelijking voor de volledige verbranding van biodiesel $\left(\mathrm{C}_{19} \mathrm{H}_{34} \mathrm{O}_{2}\right)$.
b. Schets het energiediagram voor deze volledige verbranding.

Maak bij onderstaande berekeningen gebruik van tabel 7.1 en Binas tabellen 11, 12, 28B en/of 57.
c. Onderbouw op basis van energiedichtheid (in $\mathrm{Jkg}^{-1}$ ) en met behulp van berekeningen je keuze voor de volgende brandstoffen: (bio)ethanol, biodiesel, waterstof.

Waterstof is een gas bij kamertemperatuur. Opslag gebeurt dan ook bij hoge druk of onder cryogene omstandigheden $\left(-253^{\circ} \mathrm{C}\right)$, waarbij waterstof vloeibaar is $\left(\rho_{\mathrm{H} 2}\right.$ _liq $\left.=0,070 \mathrm{~kg} \mathrm{~L}^{-1}\right)$. Dit brengt met zich mee zware en dure opslaginstallaties.
d. Onderbouw op basis van berekening je keuze voor de opslag van 1. $1,0 \mathrm{~L}$ waterstof onder hoge druk ( $700 \mathrm{bar}, 298 \mathrm{~K}$, ideaal gas);
2. $1,0 \mathrm{~L}$ waterstof onder cryogene omstandigheden;
3. 1,0 L biodiesel
e. Wat zou vanuit milieuoptiek jouw brandstofkeuze zijn? Motiveer je antwoord met 2 redenen (maak gebruik van het internet).

## Opdracht: Zonne-energie

Je ontwerpt een drone waarbij je de energievoorziening ondersteunt met zonne-energie. Het voordeel is dat je langere vluchten kunt maken, omdat je niet steeds naar het oplaadstation moet om je batterijen op te laden. Je drone vliegt namelijk op zonne-energie.

Uitgangspunt bij je ontwerp is een drone met propelleraandrijving en een elektromotor die op Lipo oplaadbare batterijen werkt. Verdere informatie staat in data-kader hiernaast en in figuur 7.6.

De vluchtduur van je oorspronkelijke drone zonder zonnecellen is beperkt door de energievoorraad aan boord (brandstof, batterij).

1. Bereken de maximale vluchtduur van je oorspronkelijke drone uitgaande van het maximum batterij-vermogen.
2. Bereken de minimale oppervlakte aan zonnecellen die je nodig hebt als het opladen van de batterijen alleen met zonne-energie gebeurt. Ga ervan uit dat je drone vliegt met maximum batterijvermogen en maak gebruik van figuur 7.6.
3. Laat aan de hand van berekening(en) zien welke overige aanpassingen je aan je drone maakt. Beschrijf ook de gevolgen (voordelen en/of nadelen) van elke aanpassing.

Je met zonnecellen uitgeruste drone vliegt nu overal heen. Nadeel is dat overdag de zon een piekintensiteit kent en 's-avonds er geen zonne-energie beschikbaar is. Dit vergt enige planning voor het effectief gebruik van de beschikbare zonne-energie.
Figuur 7.7 geeft de zonne-intensiteit weer gedurende 24 uur.
4. Maak een grafische planning, waarbij je laat zien hoeveel uren je drone bij maximaal batterijvermogen zonder tussenlanding in de lucht kan blijven. Maak hierbij gebruik van figuur 7.7.
5. Beredeneer grafisch bij welk vermogen je drone 'oneindig' lang kan doorvliegen.

## Maak en lever in:

R\&D 7 De antwoorden bij opgaven 1 t/m 5.

## Beloning:

Het goed uitvoeren van deze opdracht levert R\&D-punten op die gebruikt kunnen worden voor het ontwerp van de motor van de drone.

## Leerdoelen

Na dit hoofdstuk kun je:

- de voortstuwing van de drone relateren aan de grootheid impuls;
- het onderscheid maken tussen straal- en propelleraandrijving;
- de werking van een batterij en zijn componenten beschrijven;
- de redoxreactie uitschrijven die in een batterij plaatsvindt;
- met energiedichtheid rekenen voor het ontwerp van je drone;
- een kwalitatieve planning maken voor een drone die uitgerust is met een batterij en tevens gebruik maakt van zonne-energie.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-57.jpg?height=684&width=612&top_left_y=229&top_left_x=134)

Figuur 7.8 Een Dronegun in gebruik

## De Vliegende Rechter

## Droneshield

Bedrijven zoals Droneshield verkopen anti-drone uitrusting, zoals de "Dronegun" hiernaast. Het "vuurt" een elektromagnetische impuls die de besturingssystemen van een drone uitschakelt.

Hoewel er is een markt voor die soort uitrusting de wettelijke situatie is ver van duidelijk. In sommige landen is het uitschakelen van een drone wettelijk vergelijkbaar met het beschadigen van een vliegtuig: een ernstig delict.

## Wat denkt de Vliegende Rechter?

## VR7

a Schrijf twee brieven van minimaal 100 woorden:

- Een klachtenbrief van een persoon van wie de drone door een anti-drone geweer is vernietigd: zij/hij klaagt het bedrijf aan!
- Een antwoord van een vertegenwoordiger van het bedrijf die die uitrusting verkoopt.
b Er zijn geen bedrijven die deze dienst aanbieden in Nederland. Waarom? Geef drie onderbouwde redenen.


## 8 Vliegende Rechter: Legal Clearance

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-58.jpg?height=369&width=592&top_left_y=475&top_left_x=112)

Figuur 8.1 Het Europese parlement
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-58.jpg?height=284&width=589&top_left_y=960&top_left_x=108)

Figuur 8.2 Een veel gebruikte drone, Rob Lamping
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-58.jpg?height=467&width=589&top_left_y=1497&top_left_x=111)

Figuur 8.3 Brandend vliegtuig

## S\&B

Wil je meer leren, of hier later mee aan het werk, dan kun je de volgende opleiding overwegen:

International law
Er zijn best veel vraagtekens bij het inzetten van drones. De vorige Amerikaanse president zette veel onbemande voertuigen in tijdens gevechtsmissies. Of dit wel of niet goed is, is iets waar de meningen sterk over verschillen.

Alle voertuigen, en vooral vliegtuigen, zijn gebonden aan regels. De wet bepaalt of een auto de weg op mag en of een vliegtuig mag vliegen. Drones dus ook, met als bijkomstigheid dat het best lastig kan zijn om de verantwoordelijkheid voor de acties van een drone bij een persoon te plaatsen, vooral als het om een autonome drone gaat.

### 8.1 Wat is: ‘Legal Clearance’?

Jullie drone zal dus ook een vliegvaardigheidsbrevet moeten behalen. Het mag dan wel de snelste en meest wendbare drone zijn die er is, maar zonder vliegvaardigheidsbrevet zal het niet toegestaan zijn om ermee te vliegen. Om ervoor te zorgen dat je wel mag vliegen zul je eerst de zogeheten 'Legal Clearance' moeten krijgen. Om legal clearance te krijgen moet je:

- minimaal 70\% gescoord hebben op de opdrachten van de "Vliegende Rechter";
- de opdracht in dit hoofdstuk goed afronden.


### 8.2 Debat

Door meerdere lastige situaties en soms ernstige incidenten met drones is er momenteel een debat aan de gang over drones. Er zijn meerdere stellingen:

- Drones zijn een onacceptabel inbreuk op privacy, ze mogen alleen door bevoegde instanties gebruikt worden.
- Om incidenten op vlieghavens en andere bijzondere terreinen (bijvoorbeeld gevangenissen) te vermijden mogen alle drones die op deze terreinen terechtkomen onmiddellijk worden vernietigd.
- Gewapende autonome drones zijn een gevaar voor de samenleving.
- Niet alleen de gebruiker, maar ook de maker van een drone kan verantwoordelijk worden gesteld voor incidenten die door drones worden veroorzaakt.

Kies een stelling en een tegenstander tussen de andere teams. Als jullie de stelling verdedigen, moeten zij het aanvallen en andersom. De andere teams zullen stemmen. Let op, de leraar geeft ook punten voor feitelijk onderbouwing en logica!

## Leerdoelen

Na dit hoofdstuk kun je:

- aangeven welke belangen overheid, commercie en individuen hebben bij het gebruik van drones;
- in eigen woorden uitleggen welke maatschappelijke en wettelijke zorgpunten spelen bij drones.


## 9 Final Game of Drones

Je mag pas aan je ontwerp beginnen, wanneer je groep de legal clearance heeft gekregen van de Vliegende Rechter. Als je dit onderdeel in orde hebt, kan nu het echte werk beginnen. Dit gehele hoofdstuk zal in teken staan van de eindopdracht die in paragraaf 1 zal worden toegelicht. In tegenstelling tot eerdere hoofdstukken zal dit een R\&D eindopdracht zijn die het gehele hoofdstuk zal bevatten.

In hoofdstuk 3 tot en met 7 hebben jullie voldoende kennis vergaard over verschillende onderdelen van een drone. Daarnaast hebben jullie een ontwerpdossier bijgehouden, met daarin opgenomen:

- het programma van eisen (PvE)
- schetsen
- R\&D opdrachten
- Vliegende Rechter opdrachten

Met de R\&D opdrachten hebben jullie R\&D punten kunnen verdienen, waardoor je nu meer of minder mogelijkheden hebt bij het ontwerpen van je eigen drone. Met de R\&D opdrachten kun je nu geen punten meer verdienen.

### 9.1 Game of Drones

## GAMEDF DRONES

Ontwerp een drone waarmee je de missie (zie Casus) kan volbrengen. Zoals al eerder vermeld zal het vrijwel onmogelijk zijn om de missie met één type drone succesvol te volbrengen. Een van de belangrijke punten van een bedrijf is om te weten waar je kwaliteiten liggen, maar vooral ook waar die niet liggen. Als je er dan achter komt dat je bedrijf niet alle kwaliteiten bezit om de missie te volbrengen dan moet je allianties vormen met een of meerdere bedrijven, waardoor je samen sterker bent, en wel die missie kunt volbrengen.

Let dus op dat de strijd om de missie op dit moment nog alle kanten op kan, ook al heb je nog zo veel R\&D-punten, en daarmee extra onderdelen, verzameld.

Game of Drones nadert zijn einde. Er zijn nog drie grote opdrachten over, die zijn verdeeld over 3 paragrafen.

- 9.2 Ontwerp een Drone met specifieke eigenschappen;
- 9.3 Bedenk (gezamenlijk) een strategie hoe je de missie kunt volbrengen;
- 9.4 Verkoop je drone aan het comité.


### 9.2 Ontwerpopdracht

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-60.jpg?height=444&width=978&top_left_y=292&top_left_x=182)

Figuur 9.1 Ontwerpcyclus
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-60.jpg?height=409&width=538&top_left_y=852&top_left_x=134)

Figuur 9.2 Schetsen
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-60.jpg?height=692&width=535&top_left_y=1324&top_left_x=132)

Figuur 9.3 en 9.4 Twee verschillende drone concepten

Figuur 9.5 Definitieve ontwerpschetsen
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-60.jpg?height=475&width=538&top_left_y=2173&top_left_x=134)

In Hoofdstuk 2 zijn alle zes fasen van een ontwerpcyclus al kort voorbijgekomen. Bovendien ben je al begonnen aan fase 1, 2 en 3 . In de voorgaande hoofdstukken hebben jullie telkens aan de hand van de vergaarde kennis gekeken naar de ontwerpopdracht. Jullie zijn daardoor steeds gaan schakelen tussen fase 1,2 en 3 . In dit hoofdstuk gaan we verder met fase 3 , het bedenken van ideeën. Daarna wordt
in fase 4 een idee gekozen en uitgebreid omschreven. In fase 5 zul je je keuze moeten uitwerken in een schaalmodel/simulatiemodel. In fase 6 ga je je model testen om te kijken of het voldoet aan de missie. Kan jullie ontworpen drone daadwerkelijk (een deel van) de missie volbrengen? Hebben jullie eventueel allianties gesloten om de missie gezamenlijk te volbrengen?

## Fase 3. Ideeën bedenken

De winkel vormt de basis voor deze fase. Aan de hand van de winkel maak je keuzes per onderdeel van je drone. Bij iedere optie staan de eigenschappen van het onderdeel en de gevolgen als je voor dit specifieke onderdeel kiest. Het kan zijn dat je niet alle onderdelen mag gebruiken die in de winkel te verkrijgen zijn. Als je meer R\&Dpunten wilt hebben, kun je het comité om extra opdrachten vragen, om voor een bepaald onderdeel je score op te hogen. Laat je bij het bedenken/schetsen van je ideeën niet beperken. Zie figuur 9.2/9.3/9.4.

## Fase 4. Ontwerpvoorstel formuleren

Jullie hebben nu meerdere ideeën geschetst. Daaruit moeten jullie een keuze maken. Kies 3 concepten waarvan jullie denken dat die het best de missie kunnen volbrengen. Daarna wordt met een Harrisprofiel inzichtelijk gemaakt welk idee het best voldoet aan de eisen die jullie opgesteld hebben in het PvE. Het kan ook zijn dat het een combinatie wordt van meerdere concepten. Hierna ga je het gekozen concept verder uitwerken tot een definitief ontwerpschets. (zie figuur 9.5)

## Fase 5.Ontwerp realiseren

Met behulp van je definitieve ontwerp ga je het ontwerp realiseren door het maken van een prototype/simulatiemodel. Let op dat het niet gaat om een werkend model. In je prototype moet duidelijk zijn welke onderdelen jullie hebben gekozen, de afmetingen moeten kloppen, en de onderdelen moeten logisch op elkaar aansluiten.

## Fase 6. Ontwerp testen $\mathbb{\&}$ evalueren

De grote test. Past het, doet ie het? ledereen tevreden? Je gaat je prototype/simulatiemodel testen. Voldoet je ontwerp aan alle eisen? Zo niet, dan zul je het ontwerpcyclus (gedeeltelijk) opnieuw moeten doorlopen. Welke aanpassingen kun je maken waardoor het ontwerp wel voldoet aan alle eisen?

## R发D

## Opdracht: Eindontwerp

Fase 3: Nu je precies weet hoeveel punten je kunt uitgeven per onderdeel, kunnen jullie beginnen met maken van combinaties en het schetsen van ideeën.

Fase 4: Kies de 3 beste schetsen uit. Een Harrisprofiel kan een inzicht geven in welk van de 3 schetsen zich het best heeft gehouden aan het programma van eisen. De keuze die hieruit voortkomt werk je verder uit in een definitief ontwerp. In figuur 9.2 zie je een voorbeeld van een definitief ontwerp.

|  | schets van idee 1 |  |  |  | schets van idee 2 |  |  |  | schets van idee 3 |  |  |  |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Eis 1 |  |  |  |  |  |  |  |  |  |  |  |  |
| Eis 2 |  |  |  |  |  |  |  |  |  |  |  |  |
| Eis 3 |  |  |  |  |  |  |  |  |  |  |  |  |
| Eis 4 |  |  |  |  |  |  |  |  |  |  |  |  |
| Eis 5 |  |  |  |  |  |  |  |  |  |  |  |  |

## Stappen invullen Harrisprofiel

1. Vul de belangrijkste eisen uit het PvE in.
2. Voldoet het idee aan de eis? Kleur de vakjes: rood (negatief) of groen (positief). De hoeveelheid gekleurde vakjes bepaalt de zwaarte van de eis.
3. Doe dit voor alle drie de ideeën.
4. Bekijk het Harrisprofiel en beslis welk idee de beste keuze is. Het kan ook zo zijn dat er uit twee gecombineerde ideeën een nóg beter idee ontstaat!

Fase 5 (optioneel): Het definitieve ontwerp kan als basis dienen voor het bouwen van een prototype of een simulatiemodel.

Fase 6: Je kunt het ontwerp op veel verschillende manieren testen. Dit kan met behulp van een prototype/simulatiemodel maar ook met de tekeningen die je hebt gemaakt.

## Lever in:

1. Maak 1 of meerdere combinaties van onderdelen waarvan jullie denken dat ze (een deel van) de missie kunnen volbrengen.
2. Maak vervolgens 3 schetsen per persoon op basis van deze combinaties. Bedenk daarbij goed dat alle onderdelen in je ontwerp zichtbaar moeten zijn, maar dat je wel ontwerpvrijheid hebt in het uiterlijk van je drone.
3. Met behulp van een Harrisprofiel maak je een keuze voor je ontwerp.
4. Het gekozen idee ga je verder uitwerken tot een definitief ontwerp. Daarin moeten de volgende tekeningen worden gemaakt:

- Ruimtelijke schets;
- Kenmerkende details van je ontwerp.

5. (optioneel) Maak van je ontwerp een prototype/simulatiemodel
6. (optioneel) Simulatiemodel testen met behulp van een programma
7. Zijn er aanpassingen die je kunt maken waardoor je ontwerp nog beter tot uiting komt? Kijk nu terug naar eerdere fasen in het ontwerp.

### 9.3 Strategie

## R秉D

## Opdracht: Strategie

Het comité wil niet alleen een ontwerp zien als eindproduct, ze willen ook graag weten hoe jullie de missie gaan volbrengen.

## Lever in:

1. Bedenk nu gezamenlijk een strategie hoe je ervoor gaat zorgen dat je de missie kan volbrengen. Let daarbij op het volgende:

- Het lokaliseren van het probleem
- Het redden van de mensen en de apparatuur

Geef dit weer in tekst en beeld.

### 9.4 Presentatie

Hoe voldoet jouw ontwerp aan de gestelde eisen? Wat maakt jouw ontwerp beter dan dat van de rest? Maak een korte presentatie (max. 5 minuten) waarin je laat zien wat jouw ontwerp is, waarom je het hebt gekozen en hoe jouw ontwerp beter is dan de concurrentie. Als je hebt samengewerkt met een ander bedrijf kun je samen een presentatie geven. Je hebt dan meer tijd, maar je moet wel goed laten zien waarom jullie ontwerpen zo goed bij elkaar passen.

Je presentatie is een verkooppraatje. Dit betekent dat je je ontwerp van een positieve kant moet laten zien. Dit betekent niet dat je dingen moet aanbieden die je niet kunt leveren, dat levert namelijk dure rechtszaken op, maar wel dat je je op de positieve kanten van je ontwerp moet richten.

## 9.5 (optioneel) Politieke problemen

Een proces waarin zoveel bedrijven met elkaar concurreren, verloopt nooit helemaal vloeiend. Overheden kunnen veranderen bij tussentijdse verkiezingen, politici kunnen hun mening veranderen aan de hand van de publieke opinie. Soms kunnen bedrijven dit zelf sturen, soms kunnen dit soort dingen spontaan gebeuren. Afhankelijk
van de tijd die is uitgetrokken voor de eindopdracht kan je docent besluiten dit soort hobbels in te voeren.

Dingen die je als bedrijf kunt doen zijn bijvoorbeeld:

- De media inzetten: Geef een presentatie, waarom iets wat jij wel doet enorm belangrijk is. Aan de hand van de presentatie kan het comité besluiten de opdracht aan te passen.
- Lobby bij de overheid: Laat aan het comité weten waarom jullie de opdracht wel en anderen de opdracht niet verdienen. Jouw bedrijf heeft hard gewerkt tijdens de module en de concurrent heeft de kantjes er vanaf gelopen. Lobby bij het comité om er voordeel uit te halen.
Let op: echte lobbyisten nodigen soms potentiele klanten uit voor dure diners of geven cadeaus. Dit is natuurlijk niet de bedoeling.


## Leerdoelen

Na dit hoofdstuk kun je:

- alle fasen van de ontwerpcyclus doorlopen;
- een (concept)idee uitwerken tot een definitief ontwerp;
- terugkijken op eerdere stappen die je hebt genomen in het ontwerpproces;
- toelichten waarom je een goed ontwerp hebt gemaakt.


## Bijlage Practicum

## Practicum 1 Spaghetti

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-64.jpg?height=852&width=238&top_left_y=516&top_left_x=292)

Figuur P. 1 Spaghetti

## Inleiding

Voor je de R\&D-opdracht (brug bouwen met spaghetti) gaat doen, ga je eerst onderzoeken hoe sterk spaghetti is.

## Onderzoeksvragen

1 Hoe groot is de elasticiteitsmodulus van spaghetti?
2 Hoe groot is de treksterkte van spaghetti?

## Benodigdheden

- spaghetti (1 pak)
- een liniaal met millimeterschaal
- schuifmaat of micrometer
- statiefmateriaal en dun touw
- lijm(pistool)
- veel massablokjes (bijv. van $1 \mathrm{~g}, 2 \mathrm{~g}, 5 \mathrm{~g}, 10 \mathrm{~g}$, enz.)


## Uitvoering

Kies zelf je belastingsituatie: twee vrije steunpunten of aan een zijde ingeklemd (zie figuur 6.2).
1 Meet $L$ nauwkeurig. Zorg dat $L$ tijdens de proef niet verandert!
2 Bevestig het touwtje zo aan de spaghetti dat je er massablokjes aan kunt hangen.
De massablokjes zorgen voor de kracht $F$ die je op de spaghetti uitoefent.
3 Zet een liniaal m.b.v. statiefmateriaal zo neer dat je d kunt meten.
Meet bij elke gekozen waarde van $F$ steeds de doorbuiging $d$ zo nauwkeurig mogelijk.
4 Maak minstens acht stapjes van 2 á 5 g tot de spaghetti breekt.
5 Bepaal door meten en berekenen de waarde van het oppervlaktetraagheidsmoment $I_{0}$.
6 Bedenk zelf hoe vaak je de meetserie moet herhalen om nauwkeurig genoeg te zijn.
7 Bereken per meting de elasticiteitsmodulus $E$.

Noteer je metingen en berekeningen overzichtelijk.
Maak een diagram van het verband tussen $d$ en $F$.
Bepaal uit het diagram de elasticiteitsmodulus $E$ van spaghetti.

## Conclusie

Geef antwoord op beide onderzoeksvragen.

## Evaluatie

Geef aan welke problemen je tegenkwam en hoe je die hebt opgelost. Welke verbeteringen zijn er mogelijk in de uitvoering?

## Practicum 2 Citroenkracht?

![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-65.jpg?height=407&width=546&top_left_y=296&top_left_x=138)

Figuur P. 2 Citroenen

## Benodigdheden

- 3 citroenen
- 3 zink-elektrodes en 3 koper-elektrodes
- led-lampje
- spanningsmeter
- stroommeter


## Aanpak

1. Steek steeds een zink-elektrode en een koperen electrode in drie (halve) citroenen en verbind ze in serie met elkaar.
2. Plaats een led-lampje tussen de uiterste elektrodes waarbij je de stroomkring gesloten maakt.
3. Meet de elektrische spanning tussen de twee uiterste elektrodes en vergelijk dit met Binas tabel 48.
4. Meet nu ook de stroomsterkte die je batterij levert.
5. Vragen bij het practicum
a) Maak een schematische tekening van je opstelling en benoem de onderdelen.
b) Leid uit tabel 48 voor je citroenbatterij af welke elektrode de anode welke de kathode is.

De halfreactie die plaatsvindt aan een van de elektrodes in de citroenbatterij is: $\quad 2 \mathrm{H}^{+}+2 \mathrm{e}^{-} \rightarrow \mathrm{H}_{2}$
c) Licht toe aan welke elektrode deze reactie plaatsvindt.
d) Wat vormt de elektrolyt (zoutbrug) in je citroenbatterijen?
e) Schrijf de volledige redoxreactie uit die in de citroenbatterijen plaatsvindt.

Kan je drone nu op deze citroen vliegen? Je onderzoekt dit. Ga uit van de volgende gegevens: 1 citroen weegt 125 gram en bevat 50 mL citroensap met pH -waarde 2,30.
Ga ervan uit dat alle $\mathrm{H}^{+}$ionen bij één elektrode weg-reageren (zie ook c) en dat 1 mol elektronen correspondeert met 75 Wh .
f) Ga de waarde van 75 Wh per mol elektronen na met eerdere meting in deze proef.
g) Bereken de energiedichtheid ( $\mathrm{MJ} \mathrm{kg}^{-1}$ ) van de citroenbatterij en vergelijk dit met het Lithium-ion Polymeer batterij. Wat is je conclusie?
h) Bereken nu ook het vermogen van je citroenbatterij uit eerdere metingen in deze proef.

Een drone van $1,0 \mathrm{~kg}$ heeft een opstijgsnelheid van $2,0 \mathrm{~m} \mathrm{~s}^{-1}$.
i) Bereken hoeveel citroenen hiervoor nodig zijn. Wat is je conclusie?
j) Bedenk zelf ook een cartoonschets voor de citroenbatterij.

Maak bij het maken van onderstaande opdrachten gebruik van het internet.
k) Ga voor de Lithium-ion Polymeer batterij na wat de kathode en de anode vormt bij het ontladen.
l) Ga na wat de functie van het lithium ion is.
![](https://cdn.mathpix.com/cropped/2025_03_08_5ed077e64a86ecc6ed79g-66.jpg?height=452&width=404&top_left_y=756&top_left_x=152)

Figuur P. 3 De waterraket in drie situaties

## Practicum 3 Waterkracht ......

1. Voer vijf simulaties uit. Varieer de beginhoeveelheid water in de waterraket (0,0-1,0 kg). Stel de begindruk steeds in op 3,0 bar. - Bepaal voor elke simulatie de maximaal bereikte hoogte.
2. Zet je resultaten uit in een grafiek: op $x$-as de beginhoeveelheid water en op de $y$-as de maximaal bereikte hoogte.

- Leid uit de grafiek af de optimale watervulling bij optimale hoogte (2 decimalen).

3. Voer de simulatie nogmaals uit bij deze optimale watervulling. - Lees de optimale hoogte af en controleer met de waarde bij vraag 2.

- Leid uit de helling van de grafiek de maximale snelheid die de raket heeft.

4. Je gaat uitzoeken hoe snel de waterraket zijn maximale snelheid bereikt. Uit de grafiek lijkt dit al op $t=0$ te zijn. Is dit wel zo?

Voor het berekenen van het tijdstip ( $t_{\max }$ ) bij maximale snelheid, doe je enkele aannames en voer je een aantal deelstappen uit. Hier volgt een mogelijke stappenplan.

- Teken de krachten op de omhoogschietende raket.
- Uit de resultante kun je de versnelling (a) berekenen (neem voor je verdere berekening aan dat $a$ constant is voor het vluchtdeel waarover je de berekening uitvoert).
- Wat is de grootte van de resultante? Maak hierbij gebruik van je kennis over voortstuwing, de formules bij moduleonderdeel impuls en onderstaande formule. Neem verder aan dat het uitstromend water voor dit vluchtdeel constant is en daarmee ook de stuwkracht.

De luchtdruk in de fles veroorzaakt de snelheid waarmee het water de fles verlaat. Volgens de wet van Bernoulli geldt:

$$
v_{w}=\sqrt{\frac{2\left(p_{i n}-p_{\text {omg }}\right)}{\rho_{w}}}
$$

Hierin is:
$\boldsymbol{v}_{w}$, de snelheid van het uitstromend water ( $\mathrm{m} / \mathrm{s}$ )
$p_{\mathrm{in}}$, de druk binnenin de waterraket ( Pa )
$p_{\text {omg }}$, de druk van de omgeving ( Pa )
$\rho_{\mathrm{w}}$, de dichtheid van het water $\left(\mathrm{kg} / \mathrm{m}^{3}\right)$
5. Beredeneer, gebruikmakend van bovenstaande formule en de formule van impuls, dat de ideale beginhoeveelheid water voor een optimale maximale hoogte ergens tussen situatie I en III in ligt (figuur 7.9).
Ga er bij je redenering van uit dat bij het uitstromen van het water de luchtdruk binnenin de fles de ideale gaswet volgt en beschouw hierbij de drie situaties uit figuur 7.9.
6. Bouw in tweetallen een waterraket en voer de lancering uit waarbij je alle parameters onder vraag 2 nabootst. Meet de maximale hoogte van je vlucht en vergelijk de waarde met de waarde uit vraag 3 a . Verklaar het verschil.

## Bronnen

Link voor de "Drone no fly zones" in Nederland:
https://aeret.kaartviewer.nl/index.php?@dpf_basic\&mobiel=true\#mappage
Figuur 0.1 NOAA
Figuur 0.2 inhabitat.com/wp-content/blogs.dir/1/files/2014/02/National-Research-Center-for-
Endangered-Species-Samoo-Architects-1.jpg
Figuur 1.1 Tello Edu © roblampingfotografie
Figuur 1.2 unmannedsystemstechnology.com/2012/06/tritech-to-supply-sonar-systems-for-us-naval-auvorder/

Figuur 1.3 Dji.nl
Figuur 1.4 https://www.verenigingnlt.nl/
Figuur 1.5 btgroepi.wordpress.com/morfologische-kaart/
Figuur 1.6 bp.blogspot.com/-FF_FDx-d_e0/TuSzFFFw-kl/AAAAAAAAALg/Cfr6wYnLKVM/s320/woordweb.png (link werkt niet)

Figuur 2.1 wikipedia.org/wiki/Unmanned_aerial_vehicle
Figuur 2.2 https://www.pexels.com/photo/drone-flying-against-blue-sky-336232/ wikimedia.org/wiki/File:CopterCam3e\%2BCF30x.jpg

Figuur 2.3 money.cnn.com/2017/10/16/technology/drone-passenger-plane-canada/index.html
Figuur 3.2 www.ros.org
Figuur 3.4 www.parrot.com
Figuur 3.9 Wikipedia, Rico Shen
Figuur 4.1 Wikimedia Commons
Figuur 4.2 Wikimedia Commons
Figuur 4.3 Sparkfun.com
Figuur 4.4 Pexels.com
Figuur 4.5 Wikimedia Commons
Figuur 5.1 sciencespace.nl
Figuur 5.2 Wikipedia U.S. Air Force Photo / Lt. Col. Leslie Pratt second picture user work Zully3Cp
Figuur 5.3 Wikipedia, Theresa Knott
Figuur 5.4 Wikipedia, botag
Figuur 5.5 sam.brooks.af.mil/af/files/fsguide/HTML/Graphics/fig_28-11.gif
Figuur 5.6 Wikipedia, TSRL
Figuur 5.7 Modelbouwforum.nl
Figuur 5.8 Tello Edu © roblampingfotografie

Figuur 5.9 NASA.gov
Figuur 5.10 Fair use Boeing press material
Figuur I. 1 vwo-examen natuurkunde 2017-I
Figuur I. 2 vwo-examen natuurkunde 2017-I
Figuur 6.1 Wikimedia, CC-BY-SA-3.0
Figuur 6.5 Wikimedia, CC-BY-SA-3.0
Figuur 6.7 Wikimedia Commons
Figuur 7.1 nsastabilo.nl
Figuur 7.2 nsastabilo.nl
Figuur 7.3 zoombd24.com (link werkt niet)
Figuur 7.4 physicstasks.eu
Figuur 7.5 Wikimedia, Hazmat2
Figuur 7.6 Wikimedia, Mlino76
Figuur 7.8 Droneshield mediapackage
Figuur 8.1 Wikimedia
Figuur 8.2 © roblampingfotografie
Figuur 9.1 https://www.verenigingnlt.nl/
Figuur 9.2 CCO Commons
Figuur 9.3 CCO Commons
Figuur 9.4 CCO Commons
Figuur 9.5 designtoimprovelife.dk/wp-content/uploads/2015/06/ambulance-drone_sketches.jpg
Figuur P. 2 Wikimedia

