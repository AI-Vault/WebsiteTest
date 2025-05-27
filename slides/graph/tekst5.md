# Uitleg van de Slide: Message Passing Layer

## Inleiding
De slide bespreekt het concept van "message passing" lagen, wat een essentieel onderdeel is van grafische neurale netwerken (GNNs). Het idee is dat knopen in een netwerk informatie uitwisselen, wat helpt bij het leren en maken van voorspellingen.

## Kernconcept
- **Berichtenpassing**: Het basisidee is dat alle berichtenpassing lagen hetzelfde concept volgen, waarbij de parameter \( k \) staat voor de iteratie van het berichtenverkeer en \( v \) voor een specifieke knoop in het netwerk.
  
  De updateformule is als volgt:
  
  \[
  h^{(k+1)}_v = UPDATE(x_v, h^{(k)}_v, AGGREGATE(\{h^{(k)}_u | u \in N(v)\}))
  \]

  Hierin:
  - \( h^{(k)}_v \) is de status van knoop \( v \) op iteratie \( k \).
  - \( x_v \) is de invoerfunctie voor knoop \( v \).
  - \( N(v) \) zijn de buren van knoop \( v \), en van hen worden de berichten verzameld.

## Varianten van GNNs
De verschillende types van grafische neurale netwerken zijn afhankelijk van de keuzes die gemaakt worden voor de functies `UPDATE` en