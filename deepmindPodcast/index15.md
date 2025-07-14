# 15. Me, myself and AI ([link](https://www.youtube.com/watch?v=Ho1XPZ8JTsI))
# Samenvatting

De tekst bespreekt hoe AI-technologieën, ontwikkeld door DeepMind en gerelateerde partners, al impact hebben op diverse domeinen. Er is aandacht voor drie kerngebieden: spraaksynthese, weersvoorspellingen en voetbalanalyses.

# Spraaksynthese met Wavenet

De technologie van Wavenet wordt ingezet om menselijk klinkende stemmen te genereren via deep learning. In het verhaal wordt uitgelegd hoe DeepMind Wavenet gebruikt om stemmen te creëren die niet alleen documenten voorvisueel gehandicapten voorlezen, maar ook een natuurlijke en persoonlijke toon overbrengen.  
- Er wordt een voorbeeld getoond van hoe Wavenet de stem van Hannah Fry nabootst.  
- De techniek werkt door het modelleren van ruwe golfvormen in audio en maakt gebruik van drie fasen: tekstvoorbewerking (zoals het uitwerken van afkortingen), intonatievoorspelling, en akoestisch modelleren waarbij de identiteit van de spreker behouden blijft.  
- Er wordt ook ingegaan op fine tuning: een methode waarmee slechts enkele minuten hoogwaardige audio-opnames nodig zijn om een unieke stem nauwkeurig te reproduceren.  
- Het debat over mogelijke misbruikscenario’s komt aan bod, zoals het namaken van stemmen voor nepberichten. Er worden methoden besproken om misbruik te voorkomen, bijvoorbeeld door het niet open-sourcen van modellen en het gebruik van onhoorbare watermerken in de audio.

Een belangrijk praktijkvoorbeeld is Project Euphonia, waarbij Wavenet technologie wordt toegepast om de stem van Tim Shaw, een Amerikaanse voetballer met ALS, te reconstrueren. Dit laat zien hoe AI persoonlijke communicatie voor mensen met spraakbeperkingen kan verbeteren, al blijft het emotionele effect (herkenning van een eigen stem) een uitdaging voor zowel patienten als familie.

# Weersvoorspellingen en Nowcasting

De samenwerking tussen DeepMind en de Met Office (de Britse nationale meteorologische dienst) richt zich op het verbeteren van kortetermijnvoorspellingen (nowcasting) voor neerslag.  
- Traditionele fysische modellen voor weersvoorspelling hebben als beperking dat ze enige tijd nodig hebben voor berekeningen, terwijl nowcasting zich richt op voorspellingen tot een paar uur vooruit.  
- Oorspronkelijk werden methodes als optical flow gebruikt, maar deze gaven vaak verdoezelde (blurred) voorspellingen.  
- Met behulp van video-voorspellingsnetwerken op basis van generative adversarial networks (GAN's) kan nu realistischere en gedetailleerde voorspellingen van neerslag worden gegenereerd.  
- De gegenereerde voorspellingen worden getoetst aan werkelijke weersomstandigheden, wat aantoont dat de AI-voorspellingen qua detail en nauwkeurigheid opmerkelijk dicht in de buurt komen van de observaties.  
- Deze technologie zou in de toekomst van grote waarde kunnen zijn voor vroegtijdige waarschuwingen bij extreme regenval en overstromingen.

# AI Toepassingen in Voetbal

DeepMind onderzoekt ook hoe AI de sport voetbal kan transformeren door ondersteuning te bieden aan trainers en teams. Er worden geavanceerde technieken gebruikt om speldynamiek te analyseren en tactische beslissingen te ondersteunen:
- Er wordt gewerkt aan een “automated video assistant coach” (AVAC), een prototype dat meerdere datastromen integreert: ruwe videobeelden, trackingdata, en andere sensorgegevens.  
- Door gebruik van computer vision, game theory en statistische leermethoden kan het systeem tegenfactoriale (what-if) scenario's simuleren, zoals het verplaatsen van een speler naar een andere positie (bijvoorbeeld fabinho van verdediging naar middenveld).  
- Dit systeem biedt ondersteuning tijdens wedstrijden en bij post-match training, waarbij het moment aangeeft waarop een alternatieve beslissing, zoals een pass in plaats van een schot, mogelijk beter was geweest.  
- Er wordt ook nagedacht over het verbeteren van de ervaring voor voetbalfans door middel van gepersonaliseerde AI-commentaren, bijvoorbeeld via augmented reality of VR in het stadion.

Een uitdaging hierbij is de beschikbaarheid en kwaliteit van data. Er wordt expliciet gewezen op de discrepantie in de hoeveelheid en nauwkeurigheid van datalabels bij vrouwenvoetbal, wat aangeeft dat AI-systemen momenteel vooringenomenheden kunnen vertonen als de trainingsdata niet representatief zijn.

# Overwegingen rond Ethiek en Misbruik

De tekst belicht ook de ethische dilemma’s en mogelijke negatieve toepassingen van AI:
- Er wordt gewaarschuwd voor het risico van misbruik van tekst-naar-spraak technologie, zoals het creëren van nepnieuws of valse uitspraken, en de discussie over hoe dit tegen te gaan met toestemming en watermerken.  
- Er is een bredere discussie over de betrouwbaarheid van AI-uitvoer, aangezien mensen in de toekomst wellicht moeite zullen hebben om te onderscheiden wat authentiek is van wat door AI gegenereerd is.  
- Tot slot wordt er benadrukt dat AI-modellen slechts zo goed zijn als de data waarop ze getraind zijn, en dat het ontbreken van representatieve data tot bias kan leiden in toepassingen zoals gezichtsontgrendeling en sportanalyse.

# Conclusie

De besproken toepassingen laten zien dat DeepMind’s technologieën al een belangrijke rol spelen in diverse domeinen, van persoonlijke spraakreconstructie voor mensen met spraakproblemen tot het verbeteren van kortetermijn weersvoorspellingen en het ondersteunen van voetbalanalyses. Er wordt een hybride toekomst geschetst waarin traditionele methoden gecombineerd worden met krachtige AI-technologieën – altijd met een oog op ethische vraagstukken en de risico’s van misbruik.