# 16. Gaming, goats & general intelligence with Frederic Besse ([link](https://www.youtube.com/watch?v=64pndvbbokA))
# Belangrijke Concepten en Definitie van Agents  
Frederic Besse legt uit dat een agent in essentie een entiteit is die in een omgeving kan handelen. Dit betekent dat hij observaties ontvangt en acties onderneemt die de omgeving veranderen. Er wordt een onderscheid gemaakt tussen agent, agency (het vermogen te handelen op basis van geprogrammeerde doelen) en autonomie (het vermogen om zelfstandig beslissingen te maken en taken uit te voeren). Denk hierbij aan zowel mens als robotagenten; autopiloten in vliegtuigen vallen hier ook onder.  

# AI Agents versus Chatbots  
Er wordt besproken dat traditionele chatbots, zoals die gebaseerd op grote taalmodellen, voornamelijk werken met natuurlijke taal en een beperkte actie- of invloedssfeer hebben. In tegenstelling daaraan raken moderne agents getraind in een bredere omgeving door actief te handelen, feedback te ontvangen en op de consequenties van hun acties te leren. Hoewel taalmodellen rijk zijn aan kennis, ontbreekt hen vaak de directe mogelijkheid om fysieke of virtuele acties in een omgeving te ondernemen.

# Gebruik van Videogames als Trainingsplatform  
Videogames bieden een gecontroleerde, veilige en schaalbare omgeving waarin agents zich kunnen ontwikkelen.  
- Klassieke voorbeelden zijn de Atari-games met pixels als enige input, waar de DQN (Deep Q Network) agent leerde te handelen op basis van beloningen.  
- Complexere spellen zoals Go (met AlphaGo), schaken en Shogi (met AlphaZero) lieten zien dat agents via zelfspel en zonder menselijke data nieuwe strategieën kunnen ontdekken.  
- In realtime-strategie spellen zoals StarCraft II moeten agents optreden ondanks beperkte informatie (fog of war) en in realtime reageren.  

Deze virtuele werelden leveren rijke data op doordat ze talrijke scenario’s en omgevingen bevatten, deels door bestaande non-playable characters (NPC’s) en deels door menselijke interacties binnen de games.

# DeepMind Projecten en Nieuwe Tools  
DeepMind heeft diverse mijlpalen bereikt:
- De doorbraak met DQN voor Atari-spellen, waarin agents leerden puur op basis van pixelinformatie.
- AlphaGo en later AlphaZero, waarbij een agent zonder menselijke data een bordspel op topniveau speelde.
- De AlphaStar paper, waarin een agent StarCraft II speelde, een uitdaging gezien de partial observability en de noodzaak voor realtime beslissingen.

Daarnaast noemt Besse ook de integratie van grote taalmodellen met actuatoren via robotsystemen in papers als RT-2 en RT-X. Deze aanpak combineert wijdverspreide kennis (uit internetdata) met de mogelijkheid om fysieke acties te sturen, waardoor de kloof tussen begrip (taal) en handelen (agent actuation) wordt overbrugd.

# Het SIMA-project en Imitation Learning  
Het DeepMind-project SIMA (Scalable Instructable Multi-world Agent) richt zich op het trainen van agents die instructies kunnen opvolgen in meerdere videogame-omgevingen:
- In sandbox-spellen zoals Goat Simulator, Valheim en No Man’s Sky worden agents getraind op basis van menselijke voorbeelden in plaats van standaard beloningsmechanismen.
- Hierbij wordt gebruikgemaakt van imitation learning, waarbij het gedrag van een menselijk speler wordt nagebootst. De agents ontwikkelen hierdoor probabilistische gedragingen, zoals het nadoen van menselijke onzekerheid en het nemen van “natuurlijke” beslissingen (bijvoorbeeld het kiezen van korte routes of juist een grappige sprong maken in een spel).
- Een belangrijk resultaat is dat een agent die op meerdere spellen is getraind beter presteert in individuele spellen dan een agent die uitsluitend op één spel is getraind. Tevens blijkt dat een agent vrij goed kan generaliseren naar een geheel nieuwe, niet eerder geziene omgeving.

# Gebruikssituaties en Toekomstige AGI-toepassingen  
Het uiteindelijke doel van DeepMind is de ontwikkeling van algemeen inzetbare agents (AGI – Artificial General Intelligence) die, net als mensen, in staat zijn om zich aan te passen aan nieuwe omgevingen en omgevingen autonoom te verkennen. Voorbeelden in de toekomst kunnen onder andere zijn:
- Zelfrijdende auto's die veilig en betrouwbaar handelen in onvoorspelbare omstandigheden.
- Huisrobots of virtuele assistenten die op basis van natuurlijke taal instructies begrijpen en taken uitvoeren, zoals boodschappen doen of zware voorwerpen verplaatsen.
- Software-agents die bijvoorbeeld code kunnen schrijven of consumentonderzoek kunnen verrichten, vergelijkbaar met hoe grote taalmodellen teksten genereren, maar dan in combinatie met een actiegerichte agent die direct in een virtuele of fysieke omgeving opereert.

# Conclusie  
De gesprekken benadrukken dat videogames een cruciale en veelzijdige trainingsomgeving bieden voor de ontwikkeling van AI-agents. Door gebruik te maken van technieken zoals reinforcement learning en imitation learning, gecombineerd met natuurlijke taalverwerking, wordt er gestreefd naar agents die niet alleen in specifieke scenario’s optimaal presteren, maar ook flexibel en generaliseerbaar functioneren. Deze vooruitgang op het gebied van agents vormt een essentiële stap richting de realisatie van AGI, met brede toepassingen die variëren van geavanceerde zelfrijdende systemen tot intelligente robotassistenten in ons dagelijks leven.