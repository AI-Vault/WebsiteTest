# 4. Redefining robotics with Carolina Parada[link](https://www.youtube.com/watch?v=Rgwty6dGsYI)
# Robotica en AI-Integratie  
Het gesprek belicht hoe Google DeepMind robotica heeft getransformeerd door AI-modellen te integreren in fysieke robots. De nadruk ligt op de evolutie van traditionele robotica naar systemen die natuurlijke taal en visuele input gebruiken om complexe taken uit te voeren. Het team combineert langlopende expertise in roboticamanipulatie met de kracht van grote taal- en visuele modellen om robots meer “embodied intelligence” te geven.

# Gemini Robotics en Embodied Reasoning  
Carolina Parada bespreekt de ontwikkeling van Gemini Robotics, waarin de eerdere beperkingen van reinforcement learning voor simpele taken zijn overwonnen met de introductie van:
• LLM’s (Large Language Models) voor het begrijpen van gesproken instructies.  
• VLM’s (Visual Language Models) die de robot in staat stellen visuele context te interpreteren.  
• Transformers en multimodale modellen om niet alleen te communiceren, maar ook fysieke actie (zoals het uitvoeren van een slam dunk, het inpakken van een lunch, of zelfs het veters strikken) te genereren.  
Deze aanpak bevordert “embodied reasoning”, waarbij de robot de fysieke wereld in 3D begrijpt, objecten kan lokaliseren via bounding boxes, en intuïtief reageert op veranderende omgevingen.

# Systeem 1 en Systeem 2: Snelle Reactiviteit en Complexe Redenering  
Er wordt een duale architectuur geïntroduceerd, vergelijkbaar met Daniel Kahnemans “Thinking Fast and Slow”.  
• Het “langzame” systeem (system 2) zorgt voor complexe redenering – het interpreteert instructies, begrijpt de context van taken (zoals wat een slam dunk inhoudt) en plant een globale traject.  
• Het “snelle” systeem (system 1) is verantwoordelijk voor real-time, snelle aanpassingen op basis van visuele input en directe veranderingen in de omgeving.  
Deze combinatie maakt het mogelijk dat robots zowel doordachte als zeer reactieve acties kunnen uitvoeren, wat essentieel is voor dynamische en interactieve scenario’s.

# Interactiviteit en Teleoperatie  
Interactiviteit is een centraal thema; robots kunnen reageren op de bewegende hand van een mens of ongekende objecten in hun omgeving.  
• Er wordt gebruikgemaakt van teleoperatie en puppetry, waarbij een mens via een VR-set of direct interface de robot kan aansturen, zodat complexe handelingen getraind worden.  
• Diffusiemodellen worden ingezet om op basis van verzamelde data de benodigde actie-trajecten te voorspellen.  
Dit heeft geleid tot doorbraken, zoals het vetersstrikken en het vouwen van origami, waar eerder alleen menselijke dexteriteit voor nodig leek.

# Reinforcement Learning en Simulatie  
Hoewel de nadruk nu ligt op de integratie van grote modellen, blijft reinforcement learning een cruciaal onderdeel van robotica:  
• Robots leren basisbewegingen, zoals lopen, navigeren en objectmanipulatie, binnen gesimuleerde omgevingen.  
• De “sim-to-real gap” blijft een uitdaging, waarbij overgangen van simulatie naar de echte wereld problemen geven door verschillen in licht, dimensies en niet-gestandaardiseerde omgevingen.  
• Initiatieven zoals DemoStart demonstreren dat met slechts een paar voorbeelden (bijvoorbeeld vijf demonstraties) robots zelfstandig complexe handelingen kunnen leren door verkenning in de echte wereld.

# Veiligheid en Toepassingen in de Fysieke Wereld  
Veiligheid krijgt bijzondere aandacht door de introductie van de ASIMOV-dataset gebaseerd op Asimovs robotwetten.  
• De dataset bevat scenario’s met visuele inputs en bijbehorende veiligheidsinstructies, zoals vermijden dat een robot een glas op een instabiele plek neerzet of een object oppakt dat schade kan veroorzaken.  
• Naast softwarebeveiliging wordt er gedacht aan fysiek veilige mechanica en realtime aanpassingen, zodat robots mensvriendelijk opereren.  
Praktische toepassingen worden genoemd voor zowel thuisomgevingen, in de productie als in noodsituaties (bijv. bij natuurrampen) waar robots kunnen helpen, zelfs als er geen internetverbinding beschikbaar is.

# Nieuwe Tools en AI Workflows  
Het gesprek introduceert een aantal innovatieve workflows en tools:  
• Gemini Robotics, dat multimodale input (visuele data, taal, en nu ook acties) omzet in fysieke manipulatie.  
• Een modulair systeem bestaande uit twee AI-systemen waarbij de “zware” servergebaseerde module system 2 (denkvermogen) en de op apparaat draaiende module system 1 (reactiviteit) samenwerken.  
• Gebruik van teleoperation en VR voor het verzamelen van robotdata via menselijke ‘puppets’, aangevuld met diffusiemodellen die de actie-trajecten voorspellen.  
Deze aanpak zorgt voor een soepele integratie van AI-gebaseerde redenering en fysieke acties, wat de deur opent voor meer algemene en adaptieve robotica.

# Toekomstperspectieven en AI-Nieuws  
Er wordt voorspeld dat de komende 5 tot 10 jaar bepalend zullen zijn voor robotica. De combinatie van krachtige AI (zoals Gemini, LLM’s en VLM’s) met fysieke systemen zal leiden tot robots die complexe en niet-geprogrammeerde taken kunnen uitvoeren in onvoorspelbare omgevingen.  
• De doorbraken in embodied reasoning zullen niet alleen robotica verbeteren, maar ook de onderliggende AI-modellen versterken doordat zij beter de menselijke wereld leren begrijpen.  
• Er wordt verwezen naar een mogelijke “explosie van robotica” na de succesvolle integratie van deze AI-methoden, vergelijkbaar met de recente expansie van grote taalmodellen.

Deze innovaties en ideeën benadrukken de overgang van voorspelbare, vooraf geprogrammeerde robots naar systemen die flexibel, interactief en zelfstandig in de echte wereld opereren en menselijke vaardigheden ondersteunen en aanvullen.