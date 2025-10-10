# 40. Beyond phishing: Cyber threats in the age of AI with Four Flynn (pt. 1) ([link](https://www.youtube.com/watch?v=1gO2bC5xLlo))
# Samenvatting

• Operation Aurora en de menselijke tol  
De discussie begint met herinneringen aan de beruchte Operation Aurora, waarin een grootschalige aanval op Google in 2009 centraal stond. Flynn, die destijds actief was in de beveiligingsteams, beschrijft de intense dagen en nachten waarin hij samen met collega's (en zelfs met Sergey Brin) werkte om de aanval te identificeren, analyseren en mitigeren. Hij benoemt het enorme menselijke aspect: de stress en het gevoel van falen die erbij kwamen kijken en hoe men, ondanks de technische complexiteit van miljoenen regels code, elke kwetsbaarheid moest opsporen en verhelpen.

• Evolutie van beveiligingsmodellen: klassieke aanvalsvectoren versus Zero Trust  
Er wordt besproken hoe aanvallen in het verleden vooral op servers waren gericht via de "moat and drawbridge"-aanpak. Met de opkomst van mobiele apparaten en client-side aanvallen verschoven de bedreigingen naar kwetsbaarheden in browsers, IoT-apparaten en via social engineering. Het concept van “assume breach” en het bouwen van een layered defense, waarbij men ervan uitgaat dat een aanvaller zich al in het systeem bevindt, leidde tot de ontwikkeling van Zero Trust en BeyondCorp-benaderingen. Deze modellen richten zich op het minimaliseren van de schade nadat een inbraak heeft plaatsgevonden, door meerdere verdedigingslagen te implementeren.

• Technische kwetsbaarheden en de rol van menselijk gedrag  
De podcast belicht drie hoofdcategorieën van kwetsbaarheden:  
 – Social engineering: aanvallen waarbij de gebruiker wordt misleid (zoals phishing)  
 – Configuratiefouten: verkeerde of overmatige toegang, bijvoorbeeld door verkeerd gedeelde documenten  
 – Integriteitsproblemen: kwetsbaarheden in de code of hardware (zoals onvolledig gepatchte servers of zero-day exploits)  
Ook wordt benadrukt hoe zelfs op het niveau van IoT-apparaten (bijvoorbeeld een slim aquarium in een casino) kleine apparaten als toegangspoort kunnen dienen tot bredere netwerken en hoe belangrijk het is om met defense in depth meerdere lagen bescherming aan te brengen.

• De impact van grote taalmodellen (LLM’s) op cybersecurity  
Er wordt uitvoerig ingegaan op hoe LLM’s zoals Gemini een dubbele rol spelen in de beveiliging: enerzijds kunnen ze hun niet-deterministische gedrag, zoals variabele output bij hetzelfde invoercommando, introduceren en vatbaar maken voor prompt injectie- of jailbreak-aanvallen. Anderzijds bieden ze kansen voor verdediging en innovatie door onder meer:
 – Het versnellen van het ontdekken van kwetsbaarheden via adaptieve aanvalstechnieken, oftewel ‘adaptive attacks’, die constant proberen modellen te misleiden om potentiële backdoors te vinden.
 – Het gebruik van LLM’s om code-analyse en forensisch onderzoek te ondersteunen, waardoor een “superhuman” encyclopedische kennis van code frameworks mogelijk is.

• Nieuwe tools en AI-workflows in de verdediging  
Twee belangrijke projecten worden belicht:
 – Big Sleep: Oorspronkelijk begonnen onder de naam “project nap time” en bedoeld om kwetsbaarheden in software te detecteren. Het systeem maakt gebruik van LLM’s om code automatisch te doorzoeken – zodat beveiligingsonderzoekers “even kunnen dutten” terwijl de AI werk verricht. Big Sleep heeft al bewezen in staat te zijn om novel zero-days op te sporen, zowel in interne Google-code als in open source software.
 – Mender: Een vroege-stage project dat gericht is op het automatisch genereren van patches wanneer een kwetsbaarheid wordt ontdekt. Mender maakt gebruik van LLM’s om mogelijke oplossingen te coderen, waarbij vervolgens een reeks validatieprocessen (waaronder formele methoden en intelligent opgebouwde classifiers) wordt toegepast om ervoor te zorgen dat de automatisch gegenereerde code voldoet aan de beveiligings- en kwaliteitsnormen. Deze tool zal het makkelijker maken voor de open source community, die vaak afhankelijk is van vrijwilligers, om kwetsbaarheden snel en effectief te verhelpen.

• AI in de evolutie van zowel aanvallers als verdedigers  
Er wordt benadrukt dat AI-technologie zowel door aanvallers als verdedigers wordt ingezet. Aanvallers onderzoeken bijvoorbeeld LLM’s om malware te creëren die polymorf wordt – elke versie van de malware is anders, waardoor traditionele detectiesystemen minder effectief zijn. Tegelijkertijd benut de beveiligingsgemeenschap AI om kwetsbaarheden in enorme codebasissen te vinden voordat kwaadwillenden dat doen en om gepersonaliseerde patches te ontwikkelen. Deze strategische inzet van AI zet aan tot een toekomst waarin continue innovatie vereist is om de “defender’s dilemma” te overwinnen.

• Toekomstige ambities en de sectorale impact  
Flynn uit een ambitieus streven om theoretisch elke kwetsbaarheid in code te detecteren en automatisch te patchen, hoewel hij erkent dat er mensen- en organisatorische uitdagingen blijven bestaan – zoals de bereidheid van de wereld om patches daadwerkelijk toe te passen en legacy-systemen te moderniseren. Door transparantie te bevorderen, mede dankzij open source principes, probeert Google de beveiligingswereld als geheel vooruit te helpen. De inzet van AI als een “disinfectant” voor de industrie wordt gezien als een cruciaal onderdeel in de strijd tegen steeds geavanceerdere aanvallen, waarbij de balans tussen private en open source software een centrale rol speelt.

• Conclusie  
Het gesprek illustreert de complexe interactie tussen menselijke elementen, traditionele beveiligingsmethoden en de snel evoluerende AI-technologieën die zowel nieuwe dreigingen als nieuwe oplossingen met zich meebrengen. Door innovatieve projecten zoals Big Sleep en Mender, evenals de continue inzet om LLM’s zoals Gemini te beveiligen tegen prompt injections en andere geavanceerde aanvallen, probeert Google DeepMind met cutting-edge AI-workflows de toekomst van cybersecurity te herdefiniëren. Tevens is er aandacht voor de bredere impact van deze technologieën op zowel enterprise- als consumentbeveiliging, waarbij de verandering in de wereld van softwareontwikkeling en -beveiliging langzaam maar zeker zichtbaar wordt.