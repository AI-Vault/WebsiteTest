# Sliding Window Algorithm

## Uitleg

- **Wat is het?**  
  De sliding window algorithm is een techniek die wordt gebruikt in computer vision. Met deze techniek beweeg je een venster (of "window") over een afbeelding.

- **Hoe werkt het?**  
  Terwijl het venster over de afbeelding beweegt, vraagt het een vooraf getraind model om te bepalen of er een object aanwezig is binnen dat venster. Het model doet dit door de inhoud van dat specifieke stuk van de afbeelding te analyseren.

- **Wat zijn de resultaten?**  
  Met deze aanpak krijg je niet alleen informatie over wat er in het venster zit, maar ook de exacte locatie van het object in de afbeelding. Dit betekent dat het model "bounding boxes" kan genereren, wat rechthoeken zijn die de gedetecteerde objecten omhullen. 

## Toepassingen

Deze techniek is nuttig voor verschillende toepassingen in beeldherkenning, zoals gezichtsherkenning, verkeerssituaties en objectdetectie in autonome voertuigen.