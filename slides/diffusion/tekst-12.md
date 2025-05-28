# Uitleg van de Slide: Sampling in Neural Networks

## Notebooks
- **Doel van het Neuraal Netwerk (NN)**: Het NN heeft als doel om nauwkeurig de ruis te voorspellen die van een afbeelding moet worden verwijderd om een betere afbeelding te genereren.

## Sampling
- **Basisprincipes**: Het neuraal netwerk probeert op elke stap de ruis volledig te voorspellen. In werkelijkheid is dit echter slechts een schatting. Het vereist meerdere stappen om kwalitatief hoogwaardige afbeeldingen te verkrijgen.

- **Werkwijze**:
  1. **Noise Sample**: Een afbeelding met toegevoegde ruis wordt als uitgangspunt genomen.
  2. **Trained NN**: Een voorgetraind neuraal netwerk analyseert de ruis in de afbeelding.
  3. **Predicted Noise**: Op basis van de analyse voorspelt het NN de ruis die moet worden verwijderd.
  4. **Iteraties**: Dit proces wordt herhaald over meerdere iteraties (bijvoorbeeld ongeveer 500) om geleidelijk de kwaliteit van de afbeelding te verbeteren.

- **Visuele Representatie**: De slide toont een stap-voor-stap weergave van het proces waarbij de invoerruis en de voorspelde ruis samen met de processtappen afgebeeld zijn, wat benadrukt hoe het NN zijn voorspellingen verbetert met elke iteratie.

## Samenvatting
Het proces van sampling met een neuraal netwerk is essentieel voor het verbeteren van beeldkwaliteit door iteratief ruis te voorspellen en te verwijderen, wat leidt tot steeds betere resultaten na meerdere stappen.