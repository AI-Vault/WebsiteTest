# Uitleg van Non Max Suppression (NMS)

## Probleemstelling
In computer vision, met name bij objectdetectie, kan een algoritme meerdere begrenzingskaders (boxes) voor hetzelfde object vinden. Dit kan leiden tot onduidelijkheid over welk kader het meest geschikt is om het object te vertegenwoordigen.

## Oplossing: Non Max Suppression (NMS)
NMS is een techniek die helpt bij het filteren van overlappende boxes en het kiezen van de beste optie:

- **Selecteer de box met de hoogste kans**: Dit is meestal de box die de hoogste score heeft, vaak gebaseerd op de waarschijnlijkheid dat het object binnen de box zich bevindt.
  
- **Suppress boxes met een Intersection over Union (IOU) > 0.5**: Boxes die een hoge overlap hebben met de geselecteerde box (meer dan 50% overlap) worden onderdrukt (verwijderd) om redundantie te voorkomen.

Door deze stappen te volgen, wordt het aantal boxes dat wordt weergegeven voor een object verminderd, wat leidt tot een duidelijker en accurater resultaat in de objectdetectie.