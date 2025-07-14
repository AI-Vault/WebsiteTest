# 31. Is human data enough? With David Silver ([link](https://www.youtube.com/watch?v=zzXyPGEtseI))
# Samenvatting

Het gesprek richt zich op de ontwikkeling van AI-systemen die verder gaan dan louter het nabootsen van menselijk gedrag door menselijke data. In plaats daarvan ligt de nadruk op methoden waarbij AI-systemen door zelf ervaring op te doen leren en daarmee uiteindelijk superintelligentie bereiken. De discussie omvat onder andere het succes van AlphaGo en AlphaZero, de rol van reinforcement learning, de beperkingen van menselijke feedback, en de doorbraak in wiskundig bewijs met het systeem Alpha Proof. Hieronder volgen de belangrijkste thema’s en use cases met betrekking tot de gebruikte programma’s en tools.

## De Era van Ervaring versus Menselijke Data
- De spreker stelt dat de huidige AI-ontwikkeling grotendeels gebaseerd is op “menselijke data”. Deze methode haalt kennis uit alle menselijke bijdragen, wat aanvankelijk veel kracht oplevert.
- Om verder te gaan dan de grenzen van wat mensen kennen, moet een nieuwe aanpak worden gevolgd, namelijk de “era van ervaring”. Hierbij genereert de AI haar eigen data door interactie met de wereld en leert zij via trial-and-error. Hierdoor kan de AI buiten de beperkte menselijke kennis treden.
- Deze visie drukt een kritiek uit op het overmatig vertrouwen op menselijke feedback (Reinforcement Learning from Human Feedback – RLHF). Hoewel menselijke feedback nuttig is voor het afstemmen van antwoorden, legt het ook een limiet op de creativiteit en de mogelijkheid tot nieuwe ontdekkingen.

## Reinforcement Learning en Zelf-Verbeterende AI’s
- AlphaZero is een belangrijk voorbeeld waarbij een AI zonder menselijke data vanuit een volledig random begin via zelfspel miljoenen keren heeft geoefend en daardoor uiteindelijk superieure prestaties in spellen als Go, schaak en Shogi heeft bereikt.
- Het proces werkt op basis van reinforcement learning, waarbij een beloningsmechanisme (bijvoorbeeld +1 voor winst en −1 voor verlies) de aanpassing van het neurale netwerk stuurt. Het leert steeds nieuwe strategieën en benut zelf gegenereerde ervaring, wat resulteert in “alien moves” zoals move 37 in Go.
- Deze aanpak toont de “bittere les” van AI: menselijke kennis kan zelfs beperkend werken en het volledige potentieel van AI ondermijnen. Het verwijderen van menselijke data kan leiden tot snellere en effectievere leerprocessen.

## Alpha Proof en Wiskundige Doorbraken
- Het gesprek introduceert Alpha Proof, een systeem dat wiskundige stellingen bewijst door zelf ervaring op te doen, vergelijkbaar met hoe AlphaZero bij spellen werkt.
- Alpha Proof ontvangt duizenden menselijke geformuleerde wiskundige stellingen, maar niet de bijbehorende menselijke bewijzen. Het systeem leert via een proces van reinforcement learning, waarbij het beloningen krijgt voor correcte bewijzen en straffen voor fouten.
- Als hulpmiddel gebruikt het systeem de formele programmeertaal Lean, die alle wiskundige concepten en bewijsstructuren nauwkeurig kan formaliseren. Dit maakt het mogelijk om bewijzen te genereren die later door wiskundigen geïnterpreteerd en vertaald kunnen worden naar informele, begrijpelijke redeneringen.
- Use case: Alpha Proof behaalde een prestatie vergelijkbaar met een zilveren medaille op de International Mathematics Olympiad (IMO). Hiermee laat het zien dat AI de grenzen van menselijke wiskundige prestaties kan benaderen en zelfs kan doorbreken.

## Vergelijking tussen RLHF in LLM’s en Zelf-Lerend Vermogen
- Grootschalige taalmodellen (LLM’s) gebruiken ook reinforcement learning, maar deze systemen vertrouwen sterk op menselijke feedback om output te beoordelen. Dit zorgt ervoor dat de modellen vaak binnen de grenzen van menselijk begrip blijven en geen “alien” of geheel nieuwe ideeën ontwikkelen.
- David Silver bekritiseert deze aanpak omdat deze benadering de mogelijkheid beperkt om te ontdekken wat voor de mens nog onbekend is. Zonder de belemmering van menselijke voorkeuren kunnen AI’s potentieel nieuwe, superieure strategieën en ideeën genereren.
- Er wordt ook gesproken over het concept van “grounding”, waarbij directe, fysiek verifieerbare feedback (zoals het daadwerkelijk proeven van een cake in plaats van alleen een beoordeling van een recept) superieure leerervaringen oplevert in vergelijking met voorgeprogrammeerde menselijke voorkeuren.

## Belangrijke AI Nieuws en Toekomstige Richtingen
- Een belangrijk toekomstperspectief is om AI-systemen te ontwikkelen die zelfstandig doelen en beloningssignalen creëren op basis van complexe, soms meervoudige metriek-optimalisaties. Dit zou kunnen variëren van gezondheid (waarbij meerdere biologische en psychologische parameters in ogenschouw worden genomen) tot industriële toepassingen.
- De overstap van menselijk afgeleide data naar volledig zelfervaring-gebaseerde leerprocessen vormt een cruciaal discussiepunt binnen de AI-gemeenschap. Er wordt gewaarschuwd dat er risico’s verbonden zijn aan het loskoppelen van AI’s van menselijk toezicht, maar er zijn ook enorme voordelen wanneer AI’s steeds verder kunnen leren en verbeteren.
- De opkomst van multimodale modellen wordt genoemd als zijnde een beperkende factor, omdat zij nog te sterk geworteld zijn in menselijke data. De noodzaak om methoden te vinden die voorbijgaan aan menselijke beperkingen wordt als essentieel gezien voor de volgende fase in AI-ontwikkeling: de volledige autonomie van het leerproces.

## Ervaringen uit de Go-wereld
- Naast de technische uitleg over AlphaZero gaan de gesprekken ook in op de impact van de AI-ontwikkelingen in de Go-gemeenschap. Move 37, waarin AlphaGo een onverwachte en revolutionaire zet deed, symboliseert hoe AI’s bestaande menselijke conventies kunnen doorbreken.
- Fan Hui, de eerste professionele Go-speler die tegen AlphaGo speelde, deelt zijn ervaring van zowel verlies als het besef dat de AI zijn denkwijze had uitgebreid. Zijn perspectief benadrukt dat dergelijke doorbraken niet alleen technisch innovatief zijn, maar ook de perceptie van menselijke vaardigheden en strategieën fundamenteel veranderen.
- De interactie tussen David Silver en Fan Hui onderstreept het belang van samenwerking om zowel de ontwikkeling van de AI als de integratie ervan in menselijke domeinen te optimaliseren.

Deze uitgebreide discussie biedt inzicht in hoe reinforcement learning en ervaringen als zelfgegenereerde data de weg kunnen vrijmaken voor AI-toepassingen die ver voorbij de beperkingen van menselijke feedback reiken. Zowel in het domein van bordspellen als in de complexe wereld van wiskunde en andere echte wereld problemen, wijzen de gepresenteerde methodieken op een toekomstige fase waarin AI’s door eigen experimentatie en interactie een superieur niveau van intelligentie kunnen bereiken.