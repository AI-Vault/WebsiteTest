# Uitleg van de Slide over Graphs

## Graphs
Een graaf wordt weergegeven door de tuple \( G = (V, X_V, E, X_E) \), waarbij:
- \( V \) de knopen zijn met kenmerken \( X_V \in \mathbb{R}^{|V| \times n} \)
- \( E \) de randen zijn met kenmerken \( X_E \in \mathbb{R}^{|E| \times m} \)

### Kenmerken
- **Node features**: Dit zijn de kenmerken van de knopen, bijvoorbeeld de kleur van de knoop.
- **Edge features**: Dit verwijst naar de kenmerken van de randen, zoals de sterkte van de verbinding.

## Probleem met grafdata
1. **Verschillende invoervormen en -groottes**:
   - Grafen kunnen in grootte en structuur zeer verschillend zijn, wat consistentie in de invoer bemoeilijkt.

2. **Isomorfisme van Grafen**: 
   - Netwerken moeten in staat zijn om niet-isomorfe grafen van elkaar te onderscheiden. Dit betekent dat twee verschillende grafen die dezelfde structuur hebben, maar verschillende labels (bijvoorbeeld knoopnamen), uniek behandeld moeten worden.

3. **Netwerken moeten permutatie-invariant zijn op grafniveau**:
   - De output van een netwerk moet constant blijven bij permutaties van knopen. Het