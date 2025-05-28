# Sliding Window Algorithm

## Uitleg

- **Wanneer je de window beweegt**: Het algoritme houdt in dat je een venster (of "window") over een afbeelding schuift. Dit venster heeft een vaste grootte en kan op verschillende posities over de afbeelding worden geplaatst.

- **Getraind model beoordelen**: Terwijl je het venster verschuift, laat je een getraind model (zoals een neuraal netwerk) bepalen of er iets van belang binnen dat venster aanwezig is. Dit kan bijvoorbeeld een object zijn dat je wilt herkennen.

- **Locatie en bounding boxes**: Dit proces stelt je in staat om niet alleen te identificeren wat er in het venster zit, maar ook om de exacte locatie van het object te bepalen. Hier komen ook "bounding boxes" bij kijken, dat zijn rechthoeken rondom de gedetecteerde objecten om hun positie in de afbeelding aan te duiden.

Het sliding window algoritme is een nuttige techniek in computer vision voor objectdetectie, omdat het systematisch de afbeelding doorzoekt om objecten te vinden.