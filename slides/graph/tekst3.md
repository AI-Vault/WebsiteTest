# Uitleg over Grafen

## Grafen
Een graaf wordt weergegeven door de tuple \( G = (V, X_V, E, X_E) \), waarbij:

- \( V \) de knopen zijn met kenmerken \( X_V \in \mathbb{R}^{|V| \times n} \)
- \( E \) de randen zijn met kenmerken \( X_E \in \mathbb{R}^{|E| \times m} \)

Hierbij zijn \( n \) en \( m \) de dimensies van de respectieve kenmerken.

## Probleem met grafgegevens
- **Verschillende invoervormen en -groottes**: Grafen kunnen verschillende structuren en aantallen knopen/randen hebben, wat problemen kan veroorzaken bij de verwerking.
  
- **Isomorfisme van Grafen**: Het netwerk moet in staat zijn om onderscheid te maken tussen niet-isomorfe grafen. Twee grafen zijn isomorf als ze dezelfde structuur hebben, ook al zijn de knopen anders benoemd.

- **Permutatie-invariantie op graafniveau**: Netwerken moeten in staat zijn om de output op graafniveau invariant te maken, wat betekent dat de volgorde van knopen en randen niet uitmaakt.

- **Permutatie-equiavriantie op knooppuntniveau**: Netwerken moeten zorgen voor gelijke output wanneer de knopen op dezelfde manier worden verwisseld.

## Visuele Representatie
- **Knoopkenmerken**: De kleur van de knopen in de graf stelt verschillende eigenschappen of waarden voor.
  
- **Randkenmerken**: De sterkte van de verbinding tussen knopen, die wordt weergegeven door de gewichten van de randen in de graf.

Met deze concepten in gedachten kunnen we grafen effectiever analyseren en benutten binnen machine learning en neurale netwerken.