# U-Net Uitleg

## Wat is U-Net?
U-Net is een type neuraal netwerk dat veel wordt gebruikt voor taken zoals beeldsegmentatie. Dit betekent dat het netwerk in staat is om verschillende objecten of secties binnen een afbeelding te onderscheiden en deze afzonderlijk te labelen.

## Kenmerken van U-Net
- **Invoer- en uitvoergrootte**: Bij U-Net zijn de afmetingen van het invoer- en uitvoerplaatje gelijk (16x16x3), wat betekent dat de netwerkoutput dezelfde resolutie heeft als de ingangsafbeelding.
  
- **Downscaling en Upscaling**: Het model maakt gebruik van downscaling en upscaling, vergelijkbaar met de werking van een Variational Autoencoder (VAE).
  - **Downscaling**: Dit vermindert de dimensie van de data, waardoor een lagere dimensionale compressie ontstaat. Dit helpt bij het extraheren van belangrijke kenmerken uit de inputdata.
  - **Upscaling**: Na de downscaling wordt de afbeelding weer vergroot naar de oorspronkelijke grootte. Dit helpt om de fijne details in de output te herstellen.

## Gebruik
U-Net werd voor het eerst geïntroduceerd voor beeldsegmentatie, een belangrijke taak in computer vision, waarbij delen van afbeeldingen moeten worden geclassificeerd.

## Architectuur
De architectuur van U-Net omvat verschillende lagen:
- **Conv2D**: Convolutielagen worden gebruikt om kenmerken in de afbeeldingen te extraheren.
- **ResidualConvBlock**: Deze blokken helpen bij het behouden van informatie tijdens de diepte van het netwerk.
- **ConvTranspose2D**: Deze lagen worden gebruikt voor het upscalen van de afbeeldingsgrootte tijdens het reconstructieproces.

Overall biedt U-Net een robuuste manier om afbeeldingen te segmenteren door effectief gebruik te maken van downscaling en upscaling technieken.