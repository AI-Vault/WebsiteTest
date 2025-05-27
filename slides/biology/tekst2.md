# Uitleg over Embeddings

## Representatie van grafstructuren

- **Grote netwerken** vereisen veel berekeningen en ruimte → hierdoor zijn er technieken voor dimensionaliteitsreduktie nodig om knopen (nodes) en verbindingen (edges) te representeren.
  
- **Graph Embedding**: Grafen, knopen en verbindingen worden weergegeven als numerieke kenmerken in een laag-dimensionale ruimte.

### Toepassingen:
- **Node classificatie**: Het opleiden van modellen om te voorspellen tot welke categorie een knoop behoort.
- **Node aanbeveling**: Aanbevelen van knopen op basis van hun eigenschappen of verbindingen.
- **Link voorspelling**: Voorspellen van nieuwe verbindingen tussen knopen in het netwerk.

### Methoden:
- **Oppervlakte- of loop-gebaseerde benaderingen**: zoals Node2Vec en Path2Vec.
- **Graf Neurologische Netwerken**: Geavanceerdere technieken die gebruikmaken van de structuur van grafen om leerprocessen te verbeteren.

### Python bibliotheken:
- **NetworkX**, **DGL**, **StellarGraph**, **PyTorch Geometric**: Tools voor het werken met grafstructuren en het implementeren van verschillende methoden voor graph embedding.