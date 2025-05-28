# Diffusie: Voeg ruis toe

In deze slide wordt het proces van diffusie en het verwijderen van ruis met behulp van neurale netwerken (NN) uitgelegd.

## Fasen van het proces:

1. **Toepassing van ruis:**
   - Aan de bovenkant van de slide zie je een reeks beelden, genummerd van \( t=0 \) tot \( t=999 \). In deze reeks wordt een afbeelding geleidelijk meer verstoord door ruis naarmate \( t \) toeneemt, met \( t=0 \) als het originele beeld en \( t=999 \) als een volledige ruisversie.

2. **Neurale netwerken trainen:**
   - De slide stelt voor om daarna een neurale netwerk te trainen om op elke stap van het proces de ruis te verminderen. Dit houdt in dat het model leert de ruis te onderscheiden van het originele beeld tijdens het aanpassingsproces.

3. **Gebruik van de volledige dataset:**
   - Het neural netwerk wordt getraind met alle beelden uit de oorspronkelijke verzameling. Hierdoor kan het model generaliseren en efficiënt ruis verwijderen op basis van verschillende voorbeelden.

## Samenvatting:
Het doel van deze methode is om met behulp van neurale netwerken de ruis die is toegevoegd aan een afbeelding in verschillende stadia effectief te verwijderen, waardoor de oorspronkelijke afbeelding weer zichtbaar wordt.