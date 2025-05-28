# Uitleg van de Slide over Diffusie en Ruis

## Diffusie = Toevoegen van Gaußiaanse Ruis (Normale Ruis)

- **Gaußiaanse Ruis**:
  - Het proces van diffusie in machine learning en beeldverwerking houdt in dat er willekeurige ruis aan een afbeelding wordt toegevoegd. Deze ruis is vaak van een normale (Gaußiaanse) verdeling, wat betekent dat de meeste ruiswaarden zich rondom het gemiddelde bevinden.
  
- **Drie Kleuren**:
  - In het voorbeeld met drie kleuren wordt getoond hoe het toevoegen van ruis aan een afbeelding effect heeft op de visuele uitstraling. De afbeelding rechts illustreert dat het gebruik van meer kleuren (RGB) de perceptie van de ruis kan veranderen.

### Afbeeldingen op de Slide:

1. **16x16 Grijswaardenafbeelding**:
   - Links op de slide is er een afbeelding te zien die is gegenereerd uit een normale verdeling, weergegeven in grijswaarden. Dit is een eenvoudige representatie van ruis waaruit de fluctuaties en de willekeurigheid van de pixels zichtbaar zijn.

2. **RGB Afbeelding**:
   - Rechts zien we een afbeelding waar de ruis is toegevoegd aan een RGB-representatie met clipping, wat betekent dat sommige kleurwaarden zijn beperkt tot een bepaald bereik om te voorkomen dat ze buiten de geldige kleurnauwkeurigheid vallen.

3. **Afbeeldingen met Karakters**:
   - Onderaan de slide zijn voorbeelden van personage-afbeeldingen te zien. Deze illustreren hoe de ruis met toenemende complexiteit (of kleur) invloed kan hebben op herkenbare afbeeldingen. De afbeeldingen tonen een geleidelijke transformatie met meer ruis.

### Conclusie:

Het toevoegen van Gaußiaanse ruis is een veelgebruikte techniek in machine learning en computer vision, vooral bij het trainen van modellen om robuuster te zijn tegen ongewenste variaties in de inputdata. De voorbeelden op de slide demonstreren het effect van ruis op verschillende afbeeldingsformaten en de visuele uitwerking hiervan.