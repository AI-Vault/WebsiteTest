# Uitleg van de Slide: Intersection Over Union (IOU)

## Wat is IOU?
Intersection Over Union (IOU) is een maatstaf die wordt gebruikt om te beoordelen hoe goed een gevonden bounding box overeenkomt met een 'correcte' bounding box. Dit is vooral belangrijk in computer vision, zoals bij objectdetectie.

## Hoe werkt het?
- **Vergelijk de bounding boxes**: Je compareert de 'correcte' bounding box met de door het systeem gevonden bounding box.
- **Berekening van IOU**: IOU meet de verhouding tussen de oppervlakte van de intersectie (waar de twee boxes elkaar overlappen) en de oppervlakte van de unie (de gecombineerde oppervlakte van beide boxes).
  
  Formule:
  \[
  \text{IoU} = \frac{\text{grootte van het intersectiegebied}}{\text{grootte van het uniegebied}}
  \]

## Interpretatie
- Een IOU waarde groter dan 50% wordt als redelijk goed beschouwd.
- In de afbeelding is een voorbeeld te zien met een IOU van ongeveer 0.7899, wat betekent dat de overlap tussen de gevonden en de juiste bounding box significant is.

## Conclusie
IOU is een cruciaal concept in machine learning en computer vision, omdat het helpt bij het evalueren van de nauwkeurigheid van objectdetectiesystemen.