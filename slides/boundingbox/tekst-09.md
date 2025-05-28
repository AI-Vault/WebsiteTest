# Uitleg van de slide: Defining the target label y

## Doel van de slide
Deze slide legt uit hoe we een target label (doellabel) `y` definiëren voor een objectdetectietaak in machine learning, waarbij we verschillende typen objecten in afbeeldingen willen identificeren.

## Target labels
- **Labels**:
  - 1 - voetganger (pedestrian)
  - 2 - auto (car)
  - 3 - motorfiets (motorcycle)
  - 4 - achtergrond (background)

Deze labels worden gebruikt om de soort object in de afbeelding te categoriseren.

## Benodigde output
Voor elk object in de afbeelding moet het model de volgende informatie outputten:
- `b_x` : De x-coördinaat van de linker bovenhoek van de bounding box.
- `b_y` : De y-coördinaat van de linker bovenhoek van de bounding box.
- `b_h` : De hoogte van de bounding box.
- `b_w` : De breedte van de bounding box.
- Klasse label (1-4): Het label dat aangeeft tot welke categorie het object behoort.

## Afbeeldingen
Aan de rechterkant van de slide zijn er twee afbeeldingen:
- De linker afbeelding toont een voertuig met een bounding box.
- De rechter afbeelding toont een achtergrond zonder objecten van belang.

## Vraag op de slide
De slide bevat twee vragen:
1. Hoe eerder de labels zonder bounding box zijn gedefinieerd.
2. Hoe deze aanpak gegeneraliseerd kan worden, wat impliceert dat het model moet kunnen leren om niet alleen specifieke objecten, maar ook verschillende variaties en nieuwe objecten te identificeren in ongekende contexten.

## Conclusie
De slide benadrukt de noodzaak van duidelijke labeling en het vermogen van het model om te generaliseren, wat cruciaal is voor de effectiviteit van objectdetectie in machine learning.