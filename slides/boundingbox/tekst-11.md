# Uitleg van de slide: Definiëren van het doellabel y

In deze slide wordt uitgelegd hoe het doellabel, aangeduid als \( y \), wordt gedefinieerd voor een machine learning model dat zich richt op objectdetectie. Hier zijn de belangrijkste elementen:

## Doelclassificatie

We hebben vier mogelijke klassen:

1. **1 - voetganger**
2. **2 - auto**
3. **3 - motorfiets**
4. **4 - achtergrond**

Deze klassen geven aan wat voor type objecten het model moet identificeren in de afbeeldingen.

## Benodigde output

Het model moet verschillende waarden teruggeven, waaronder:

- \( b_x, b_y, b_h, b_w \): Dit zijn de coördinaten en afmetingen van de "bounding box" die het object omringt:
  - \( b_x \): x-coördinaat van de linkerbovenhoek van de bounding box.
  - \( b_y \): y-coördinaat van de linkerbovenhoek.
  - \( b_h \): hoogte van de bounding box.
  - \( b_w \): breedte van de bounding box.

- **Klasse-label (1-4)**: Dit label geeft aan welk type object is gedetecteerd in de afbeelding.

## Voorbeeld

De afbeeldingen van het model tonen aan hoe deze werkprocessen functioneren:

- **Eerste afbeelding**: Hier detecteert het model een auto. De pandingsbox coördinaten en dimensies worden weergegeven, samen met het klasse-label (bijvoorbeeld \( 2 \) voor auto).

- **Tweede afbeelding**: Dit is een afbeelding van een achtergrond zonder een herkenbaar object. Hier is het klasse-label ingesteld op "0" (bijvoorbeeld "maak je niet druk"), wat aangeeft dat er geen relevant object is.

## Samenvatting

De slide legt duidelijk uit hoe een systeem moet werken om objecten in afbeeldingen te identificeren en waar te nemen door middel van objectdetectie. Door het gebruik van bounding boxes en klasse-labels kan het model de aanwezigheid van verschillende objecten onderscheiden en classificeren.