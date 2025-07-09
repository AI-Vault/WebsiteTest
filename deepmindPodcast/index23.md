# 23. Me, myself and AI ([link](https://www.youtube.com/watch?v=Ho1XPZ8JTsI))
# Overzicht van DeepMind Podcast aflevering "Me, Myself and AI"

Deze aflevering behandelt meerdere toepassingen van AI, met een focus op hoe DeepMind’s technologieën al impact hebben in de echte wereld. Er komen onderwerpen aan bod zoals spraaksynthese, weersvoorspellingen en voetbalanalyse, en er wordt uitgebreid stilgestaan bij de uitdagingen, ethische implicaties en toekomstige potentie van deze toepassingen.

# Spraaksynthese met WaveNet

• De aflevering start met een demonstratie van WaveNet, een spraaksynthesetechnologie die deep neural networks gebruikt om menselijke stemmen na te bootsen.  
• Er wordt uitgelegd hoe WaveNet werkt: in plaats van het samenvoegen van vooraf opgenomen fragmenten, modelleert het direct de ruwe geluidsgolf met een tijdsinterval van minder dan een milliseconde.  
• Toepassingen:  
  - Het creëren van natuurlijke stemmen voor podcasts, smart speakers en voor mensen met visuele beperkingen.  
  - Het reconstrueren van stemmen voor mensen met spraakstoornissen, zoals in het geval van Tim Shaw, een atleet met ALS, wiens stem door AI opnieuw werd gegenereerd zodat hij zijn stem kon horen na stemverlies.  
• Workflow:  
  - Het verzamelen van hoge kwaliteit audio-opnames (ongeveer 10 minuten) gekoppeld aan transcripties wordt gebruikt om de AI te trainen.  
  - Een proces genaamd “fine tuning” maakt het mogelijk om individuele stemkenmerken nauwkeurig te modelleren met slechts enkele minuten sample-audio.  
• Ethische aspecten:  
  - Het belang van toestemming voor het gebruiken van iemands stem.  
  - Overwegingen rond misbruik en de plannen voor watermerken in audio om te onderscheiden of een opname echt of gesynthetiseerd is.

# AI in Weersvoorspelling: Now Casting

• DeepMind werkt samen met het Britse Met Office om AI-gestuurde korte termijn weersvoorspellingen (“now casting”) te verbeteren.  
• Toepassing:  
  - Het voorspellen van regenval en de beweging van weerssystemen op een hogere resolutie, zodat uitdijende weersfenomenen zoals overstromingen beter kunnen worden voorspeld.  
  - Deze korte termijn voorspellingen ondersteunen evacuatieplannen en andere noodmaatregelen bij extreem weer.  
• Technieken en Workflow:  
  - Traditionele methoden zoals optical flow (een computervisie techniek) worden gecombineerd met deep learning.  
  - Video prediction: AI voorspelt de volgende frames van een “weervideo”, waarin radarbeelden van regenval worden gebruikt.  
  - Een Generative Adversarial Network (GAN) wordt ingezet: twee netwerken concurreren (een generator en een discriminator) om zeer realistische voorspellingen te genereren met scherpe, gedetailleerde structuren van neerslag.  
• Resultaten en uitdagingen:  
  - De AI levert nu-casting voorspellingen die erg overeenkomen met de werkelijkheid, maar heeft moeite met het voorspellen van uitzonderlijke en extreme weersomstandigheden.  
  - Er wordt gekeken naar een hybride aanpak: het combineren van traditionele fysisch gebaseerde modellen met deep learning om nauwkeurigere voorspellingen te genereren.

# AI in Voetbal: Automated Video Assistant Coach (AVAC)

• DeepMind werkt samen met Liverpool Football Club aan toepassingen van AI in de sportanalyse.  
• Doel en use cases:  
  - Ontwikkelen van een AVAC-systeem dat meerdere datastromen (zoals video-opnames, tracking data, sensorgegevens en evenementstromen) combineert om coaches real-time tactische inzichten te geven.  
  - Het systeem kan “what-if” scenario’s simuleren, bijvoorbeeld het effect van een positiewisseling van spelers, en voorspelde spelersbewegingen visualiseren.  
  - Post-match analyses: Het systeem kan in video’s aangeven wanneer een betere tactische beslissing had kunnen worden genomen, zoals een pass in plaats van een schot op doel.  
• Gebruikte technologieën:  
  - Computervisie voor het analyseren van videobeelden tijdens wedstrijden.  
  - Speltheorie en statistische methoden voor het ontdekken van patronen in historische wedstrijden.  
• Uitdagingen en bredere implicaties:  
  - Er zijn zorgen over bias in AI-systemen, zoals de verminderde accuraatheid bij het analyseren van videomateriaal in vrouwenvoetbal door een gebrek aan voldoende geannoteerde trainingsdata.  
  - Het accent ligt op het ondersteunen van menselijke beslissingen, zonder de rol van de coach of spelers volledig over te nemen.

# Conclusie

De aflevering laat zien hoe AI op verschillende fronten – van spraak tot weersvoorspelling en sport – wordt ingezet om zowel problemen met persoonlijke impact als wereldwijde toepassingen aan te pakken. Er wordt daarbij niet alleen gekeken naar technische vooruitgang en gebruiksscenario’s, maar ook naar de ethische vraagstukken die gepaard gaan met deze ontwikkelingen. Nieuwe tools zoals WaveNet, video prediction met GAN’s en hybride modellen voor now casting illustreren de versnelling in AI-innovaties, terwijl samenwerkingen met organisaties als het Britse Met Office en Liverpool FC aangeven hoe breed en veelzijdig de impact van AI inmiddels is.