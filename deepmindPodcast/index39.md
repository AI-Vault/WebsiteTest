# 39. Genie 3: An infinite world model with Shlomi Fruchter and Jack Parker-Holder ([link](https://www.youtube.com/watch?v=n5x6yXDj0uo))
# Samenvatting

Deze uitgebreide tekst gaat over een nieuw interactief wereldmodel dat bekend staat als Genie3. Het centrale thema is het ontwikkelen van een neurale netwerksimulatie die in real time een dynamische, interactieve wereld op basis van een tekst- of beeldprompt genereert, zonder gebruik te maken van een traditionele game-engine.

## Belangrijke onderwerpen en thema's

• Er wordt besproken hoe innovaties – zoals de evolutie van video- en beeldgeneratiemodellen – steeds meer mogelijkheden bieden om omgevingen te simuleren die niet alleen visueel realistisch zijn, maar ook interactief en consistent ervaren kunnen worden.  
• Er wordt benadrukt dat veel technologische doorbraken, zoals het creëren van geheel nieuwe omgevingen, niet vaak als doel zijn gestart, maar eerder als emergente eigenschappen van een breed getraind model.  
• De discussie gaat dieper in op de noodzaak van simulatie voor het trainen van agents en robots in veilige, gecontroleerde omgevingen, zodat zij in de echte wereld robuust gedrag kunnen tonen, zonder de risico’s die directe experimenten met fysieke systemen met zich meebrengen.  
• Verder wordt het idee aangekaart dat het loslaten van agents zonder duidelijke doelstellingen – een aanpak waarin mensen bepalen wat interessant is – tot onverwachte, creatieve doorbraken kan leiden, vergelijkbaar met hoe de evolutie van de wiskunde en kunst tot nieuwe inzichten heeft geleid.

## Toepassingen en gebruiksscenario’s

• Training van agents: Genie3 kan gebruikt worden als simulatieomgeving om embodied agents of robotica veilig te trainen. Hierbij kan men de simulatie inzetten voor het testen, evalueren en aanpassen van gedrag van agents in uiteenlopende, vaak uitdagende situaties.  
• Planningsstrategieën: Agents kunnen in de gegenereerde wereld scenario’s uitproberen (bijvoorbeeld een robot die een weg moet oversteken) om via rollouts een reeks mogelijke acties te evalueren.  
• Educatieve toepassingen: Door virtuele werelden te creëren (bijvoorbeeld een herinterpreteerde versie van een historische locatie, zoals Victorian England of een schilderij als Edward Hopper’s Nighthawks), biedt deze technologie een unieke manier van leren en ervaringsgerichte educatie.  
• Entertainment en simulaties: Naast traditionele games wordt er ook nagedacht over toepassingen in recreatieve ervaringen, zoals interactieve tours, simulaties van exotische experiënties (bv. jet ski varen langs eilanden), en potentieel zelfs therapeutische toepassingen, zoals het herbeleven van herinneringen voor mensen met dementie.

## Gebruikte programma’s, tools en AI-workflows

• Het model genereert elke pixel in de omgeving door autoregressieve voorspelling. Dit betekent dat hver frame wordt berekend op basis van de voorafgaande input, vergelijkbaar met hoe taalmodellen het volgende woord voorspellen.  
• Er wordt gebruikgemaakt van transformerarchitecturen die zowel in taalmodellen als in beeld- en videomodellen centraal staan.  
• De workflow combineert text-to-image en text-to-video benaderingen met auto-regressieve generatie voor real-time simulatie. Door gebruik te maken van promptable world events kan de gebruiker “on the fly” objecten of gebeurtenissen toevoegen aan de gegenereerde omgeving, wat zowel voor menselijk entertainment als voor agent training van belang is.  
• Er is een evolutie zichtbaar van eerdere iteraties (Genie1 en Genie2) waarbij de schaal, consistentie en interactiviteit stap voor stap werd uitgebreid. Genie1 bood eerst een 2D, beperkte omgeving, die in Genie2 opgeschaald werd naar 3D en hogere resolutie.

## Nieuwe AI-workflows en emergente eigenschappen

• Emergent gedrag: Het model vertoont opmerkelijke ‘emergente eigenschappen’, zoals het correct simuleren van natuurkundige effecten (waterstoten, zwaartekracht, vochtige omgevingen) zonder dat dit expliciet in de regels geprogrammeerd was.  
• Autoregressieve simulatie: Elke frame wordt gegenereerd uit de ‘geheugen’ van de voorgaande frames, wat resulteert in een consistente wereld en een realistisch naslagwerk van de omgeving, zelfs als de gebruiker van hoek verandert.  
• Flexibele input: Zowel tekst prompts als afbeeldingen en video's kunnen als startpunt dienen om een interactieve en beschrijvende omgeving te genereren.  
• Verbeterde consistentie: De nieuwe modellen onthouden reeds gegenereerde details zodat bij terugkieken in een scene dezelfde elementen behouden blijven. Dit werkt samen met de mogelijkheid voor agenten om door de wereld te navigeren en daarbij constante omgevingskenmerken te ervaren.

## AI-nieuws en bredere context

• Het gesprek plaatst Genie3 in de bredere context van AI-onderzoek en AGI (Artificial General Intelligence). De sprekers benadrukken dat een echte AGI nood heeft aan een simulatie van de fysieke wereld zodat agents kunnen leren en op een veilige manier experimenteren.  
• Er wordt gewezen op de snel evoluerende aard van generatieve modellen, waarin eerdere beperkingen (zoals foutieve beeldgeneratie, bijvoorbeeld bij menselijke handen) al snel zijn opgelost.  
• Er wordt nagedacht over de ethische en veiligheidsimplicaties, zoals het vermijden van ongewenste geweldsscènes of onbruikbare scenario’s in zowel simulaties als trainingen van agents, met een focus op feedback en gecontroleerde vroege toegang om risico’s in te perken.  
• Tot slot komt het idee naar voren dat domein-randomisatie (het invoeren van willekeurige variaties om agents robuuster te maken) een belangrijk aspect is om de kloof tussen simulatie en realiteit te verkleinen.

Deze doorbraken in het genereren van doorlopende, interactieve en consistente omgevingen vormen een belangrijke stap richting systemen die kunnen plannen en redeneren — een cruciale voorwaarde voor een toekomstige, embodied AGI.