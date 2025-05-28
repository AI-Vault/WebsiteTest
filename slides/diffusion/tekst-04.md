# Uitleg van de Slide over Diffusie en Gaussian Noise

## Diffusie = toevoegen van Gaussian noise (= Normaal Geluid)
- **Gaussian noise**: Dit verwijst naar pixelwaarden die zijn afgeleid van een normale verdeling. Dit type ruis wordt vaak gebruikt in machine learning en beeldbewerking om verschillende effecten te bereiken, zoals het verbeteren van de robuustheid van modellen.

### Python Code

De slide bevat een stuk Python-code dat het proces van het genereren en visualiseren van Gaussian noise in een 16x16 dimensie illustreert.

1. **Array Genereren**:
   ```python
   array = np.random.normal(loc=0.5, scale=0.35, size=(16, 16))
   ```
   Hier wordt een 16x16 array gegenereerd met waarden vanuit een normale verdeling, waarbij `loc` het gemiddelde (0.5) en `scale` de standaardafwijking (0.35) vertegenwoordigt.

2. **Knippen van Waarden**:
   ```python
   array_clipped = np.clip(array, 0, 1)
   ```
   Dit zorgt ervoor dat alle waarden in de array worden beperkt tot het bereik van 0 tot 1.

3. **Schaal naar Grijswaarden**:
   ```python
   image = (array_clipped * 255).astype(np.uint8)
   ```
   De waarden worden geschaald naar een bereik van 0-255 om een grijswaardenafbeelding te creëren.

4. **Afbeelding Tonen**:
   ```python
   plt.imshow(image, cmap='gray', vmin=0, vmax=255)
   plt.axis('off')
   plt.title("16x16 Grayscale Image from Normal Distribution")
   plt.show()
   ```
   Deze code toont de afbeelding op een grijswaardenkleurenschema, zonder assen.

### Grafieken

- Aan de rechterkant van de slide zie je een histogram. Dit toont de verdeling van de waarden in het gegenereerde array, samen met een normale verdeling (de rode lijn).
- De histogram geeft weer hoe vaak waarden voorkomen in het array in vergelijking met de theoretische normale verdeling.

## Conclusie
De slide illustreert hoe Gaussian noise kan worden toegevoegd aan beelden door middel van Python, en laat zien hoe de resulterende waarden de normale verdeling volgen. Dit is een belangrijk concept binnen machine learning, vooral bij het trainen van neurale netwerken.