# Uitleg van de Slide: Diffusion - Voeg Ruis Toe

## Inleiding
Deze slide legt een concept uit dat veel wordt gebruikt in machine learning en computer vision, vooral in het kader van generatieve modellen en ruisverwerking, genaamd "diffusie". 

## Visuele Weergave
De afbeeldingen bovenaan de slide tonen hoe er na verloop van tijd ruis aan een oorspronkelijke afbeelding wordt toegevoegd. Elke afbeelding is genummerd met een tijdstap (t=0, t=100, t=200, enzovoort). 

### Tijdstappen
- **t=0:** Dit is de oorspronkelijke afbeelding zonder ruis.
- **t=100 tot t=900:** In deze beelden wordt geleidelijk meer ruis toegevoegd. Men kan zien dat de beelden steeds minder herkenbaar worden naarmate de tijdsduur toeneemt.
- **t=999:** Op dit punt is de afbeelding praktisch onherkenbaar of volledig verstopt door ruis.

## Onderste Regel
- **"Voeg steeds meer ruis toe in bijv. 1000 stappen":** Dit geeft aan dat het proces van het toevoegen van ruis in kleine stappen gebeurt, bijvoorbeeld in 1000 iteraties. Dit helpt om een gecontroleerde overgang naar volledig ruizige beelden te creëren, wat nuttig kan zijn voor het trainen van modellen in generatieve taken.

## Conclusie
Het toevoegen van ruis door het diffusieproces helpt bij verschillende machine learning-toepassingen, zoals het verbeteren van generatieve modellen en het leren van robuuste representaties. Het laat zien hoe afbeeldingen evolueren van een heldere, herkenbare staat naar een meer chaotische toestand door de impact van ruis.