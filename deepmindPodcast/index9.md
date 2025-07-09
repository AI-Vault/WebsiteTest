# 9. Gemini 2.0 and the evolution of agentic AI with Oriol Vinyals ([link](https://www.youtube.com/watch?v=78mEYaztGaw))
# Samenvatting

De podcast bespreekt de evolutie van agent-gebaseerde systemen binnen de AI, waarbij Oriol Vinyals van Drastic Research en co-tech-lead van Gemini uitlegt hoe deze systemen sinds 2019 gegroeid zijn en wat de huidige stand van zaken is.

# Trainingsmethodologie en Architectuur
• Er wordt een tweestapsproces beschreven dat al sinds AlphaGo en AlphaStar wordt gebruikt.  
 – Eerst vindt een pretraining of imitatie-leren plaats, waarbij een model traint op grote hoeveelheden menselijk geproduceerde data (bijv. het internet) om menselijke patronen na te bootsen.  
 – Daarna volgt een reinforcement learning (post-training) fase, waarin het model leert aan de hand van beloningssignalen (zoals winnen of het schrijven van een “goed” gedicht) om de prestaties te verfijnen.  
• De onderliggende architectuur is geëvolueerd van vroege algoritmes zoals DQN naar transformer-gebaseerde modellen. Kleine tweaks in het netwerk (laag aantallen, breedte van lagen, verwijdering van onnodige neuronen) kunnen een grote impact hebben op de prestaties.

# Schaalvergroting en Data-uitdagingen
• Hoewel schaalvergroting (meer neuronen & parameters) de prestaties verbetert, leidt dit tot afnemende rendementen op de lange termijn, wat vergelijkbaar is met het opruimen van een rommelige kamer: aanvankelijk is er veel verbetering, maar na verloop van tijd levert een extra kleine optimalisatie weinig op.  
• Er is een eindige hoeveelheid beschikbare data, waardoor technieken zoals synthetische data worden onderzocht om de trainingsdata te vergroten en de grenzen van de huidige schalingswetten te doorbreken.

# Multimodale Modellen en Brede Toepassingen
• Huidige grote taalmodellen zijn multimodaal, wat betekent dat ze niet alleen tekst, maar ook afbeeldingen en video’s kunnen verwerken.  
• Deze modellen vormen nu de centrale “elektrische brein” waarop verdere, agentische toepassingen gebouwd kunnen worden.  
• De “Gemini 1.5 Flash” is een voorbeeld van een set bevroren gewichten die na een intensief trainingstraject niet meer worden aangepast, terwijl Gemini 2.0 generatieve en agentische verbeteringen biedt.

# Integratie van Externe Tools en Agentisch Gedrag
• Om meer agentisch gedrag te bereiken, worden de centrale modellen omgeven met “digitale lichamen”. Dit betekent dat ze naast hun interne berekeningen externe hulpmiddelen kunnen aanroepen, zoals:
 – Een geïntegreerde zoekmachine (zoals Google Search) voor actueel nieuws of informatie.  
 – Mogelijkheden om code uit te voeren of een browser te besturen om taken automatisch af te handelen (bv. het vinden van hotels, reizen plannen).  
 – Integratie in Chrome als een companion-agent die routinetaken kan automatiseren door acties zoals klikken en navigeren op websites over te nemen.
• Dit creëert nieuwe workflow mogelijkheden, zoals het automatisch doorzoeken van nieuwsartikelen, het samenvatten van content en zelfs het spelen van spellen via een webinterface, wat een brug slaat tussen traditionele spelsystemen en algemene AI-vaardigheden.

# Redeneren, Planning en Werkgeheugen
• De modellen beginnen zich te ontwikkelen richting complexer redeneren en planning:
 – Ze kunnen meerdere stappen ondernemen, zoals het eerst samenvatten van tientallen artikelen en vervolgens de informatie clusteren om een finale, op maat gemaakte samenvatting te geven.  
 – Dit vergt een soort “werkgeheugen” waarin tijdelijke notities of “scratchpads” worden gebruikt.  
• De drie vormen van geheugen binnen deze systemen worden besproken:
 – Het langetermijngeheugen in de vorm van voorgetrainde gewichten (alles wat ze hebben geleerd).  
 – Episodisch geheugen, bijvoorbeeld door toegang te krijgen tot externe zoekresultaten of historische data.  
 – Werkgeheugen (context van duizenden tokens) dat ingezet kan worden voor complexe redenerings- en planningsprocessen.

# Toepassingen en AI Workflows
• Er wordt veel aandacht besteed aan praktische toepassingen zoals:
 – Automatisering van repetitieve of triviale taken in de browser (reizen boeken, agenda checken, etc.) via een agent die intuïtief kan navigeren en klikken.  
 – Software engineering, waarbij de AI niet alleen code schrijft, maar deze ook kan testen en iteratief verfijnen op basis van feedback.  
 – Spelgerelateerde toepassingen, zoals een agent die een spel speelt, advies geeft of als game companion fungeert.
• Deze workflows vormen belangrijke stappen richting bredere, generalistische intelligentie, waarbij de modellen niet enkel voorspellingen doen op basis van hun trainingsdata, maar ook zelfstandig acties ondernemen en leren van nieuwe ervaringen.

# AI Nieuws en Toekomstperspectieven
• De discussie benadrukt dat de huidige technologische vooruitgang (zoals Gemini 2.0) de weg vrijmaakt voor steeds meer “agentische” capaciteiten en richting AGI gaat.  
• Er wordt gewaarschuwd voor uitdagingen, zoals de beperkingen van beloningsmodellen bij subjectieve taken (bijvoorbeeld het beoordelen van een gedicht) en de risico’s van bias wanneer modellen eigen output als trainingsdata gebruiken.  
• De vooruitzichten zijn optimistisch: de combinatie van schaalvergroting, geavanceerde architecturen, integratie van externe tools en verbeterd geheugen en redenering kan leiden tot AI-systemen die superieure prestaties leveren in domeinen met duidelijke “ground truth” (zoals wetenschap en protein folding).

Kortom, de podcast biedt een diepgaande blik op de evolutie van AI-agenten, de technische uitdagingen van schaalvergroting en data, en de integratie van digitale lichamen die autonome handelingen kunnen verrichten – een cruciale stap richting meer algemene en wellicht superieure intelligentie.