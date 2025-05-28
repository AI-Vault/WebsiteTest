# Intersection Over Union (IoU)

## Inleiding
Intersection Over Union (IoU) is een belangrijke maatstaf in computer vision, vooral in objectdetectietaken. Het helpt te bepalen hoe goed een gevonden bounding box (de rechthoek die een object omringt) overeenkomt met de werkelijke locatie van dat object.

## Hoe werkt het?
Met IoU meet je de overlap tussen de voorspelde bounding box en de werkelijke bounding box. 

1. **Berekening van de area**:
   - **Intersection**: Dit is het gebied waarin de voorspelde bounding box en de werkelijke bounding box elkaar overlappen.
   - **Union**: Dit is het totale gebied van beide bounding boxes samen (van de combinatie van beide).

2. **Formule**:
   \[
   IoU = \frac{\text{Intersection}}{\text{Union}}
   \]
   - Een hogere IoU-score (bijvoorbeeld > 0.5) duidt op een betere overeenkomst tussen de twee bounding boxes.

## Visualisatie
In de bijgevoegde afbeelding zie je een voorbeeld:
- Er is een afbeelding van een weg met een auto.
- De rode rechthoek toont de voorspelde bounding box van de auto.
- De blauwe grid geeft een context aan de omgeving.

## Belang
IoU is essentieel voor het trainen van modellen en het evalueren van hun prestaties. Hoe beter de IoU, hoe betrouwbaarder het model in het detecteren van objecten in beelden.

---

Door het gebruik van IoU kunnen ontwikkelaars en onderzoekers de effectiviteit van objectdetectiemodellen verbeteren en optimaliseren.