# Uitleg van de Slide over Diffusie en Neural Networks

## Diffusie: Voeg Ruis Toe

### Visualisatie
- Bovenaan de slide zien we een reeks beelden die de progressie van een afbeelding met toegevoegde ruis op verschillende tijdstippen (t=0, t=100, ..., t=999) weergeven.
- De eerste afbeelding (t=0) toont een helder beeld, terwijl het beeld steeds ruisiger wordt naarmate de tijd vordert (tot t=999).

### Training van een Neural Network
- **Train vervolgens een Neural Net:** Het doel is om een neural network te trainen dat in staat is om de ruis van een afbeelding in elke fase te verwijderen.
- Voor elke stap wordt de neural net getraind om de afbeelding te de-noisen, zodat het oorspronkelijke, heldere beeld (t=0) weer zichtbaar wordt.

### Gebruik van de Trainingsdata
- **Je traint dit met alle plaatjes uit je beginverzameling:** Dit houdt in dat de neural nets getraind worden met de verschillende versies van de afbeeldingen met ruis, zodat ze leren hoe ze de ruis kunnen verminderen voor elke fase van t.

### Vraag
- **Hoe kan je nu plaatjes van paarden genereren?** Dit suggereert een toepassing van het getrainde neural network, mogelijk om nieuwe, synthetische beelden van paarden te creëren op basis van de aangeleerde ruisverwijzing. 

## Conclusie
Deze slide legt uit hoe diffusie wordt toegepast binnen een neural network context, waarbij ruis wordt toegevoegd en vervolgens door een getraind netwerk wordt verwijderd. Het biedt een basis voor verdere toepassingen in beeldgeneratie.