## Grafen

### Representatie van een graaf:

- Een graaf wordt weergegeven door de tupel \( G = (V, X_V, E, X_E) \), waarbij:
  - \( V \) de knopen zijn met kenmerken \( X_V \) met dimensies \( \mathbb{R}^{|V| \times n} \)
  - \( E \) de randen zijn met kenmerken \( X_E \) met dimensies \( \mathbb{R}^{|E| \times m} \)

### Probleem met graafdata:

- **Verschillende invoervormen en -groottes**: De data van grafen kunnen sterk variëren in structuur en formaat.
  
- **Isomorfisme van grafen**: Het netwerk moet in staat zijn om niet-isomorfe grafen te onderscheiden, d.w.z. grafen die niet identiek zijn ondanks een soortgelijke structuur.

- **Permutatie-invariantie op graafniveau**: Netwerken moeten een output geven die niet verandert als knopen of randen binnen de graaf permuteren.

- **Permutatie-equivalentie op knoopniveau**: Dit betekent dat als we de volgorde van knopen veranderen (permutatie), de output overeenkomstig moet veranderen op een voorspelbare manier, maar in dezelfde relatie tot de permutaties van de invoer.

### Kenmerken van de grafiek:

- **K