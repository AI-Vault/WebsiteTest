# Uitleg van de slide: Vroegste voorbeelden van recurrente GNN's

## Basisconcept
De slide behandelt de eerste voorbeelden van recurrente graf-neurale netwerken (GNN's), die zijn gebaseerd op het idee van een recurrent netwerk. 

- **UPDATE en AGGREGATE:** Deze twee functies zijn hetzelfde voor elke iteratie van de berichtoverdracht in het netwerk. Dit betekent dat de wijze waarop informatie wordt bijgewerkt en geaggregeerd, consistent blijft gedurende het proces.

## Formule
De kernformulier is gegeven als:
\[ h_v^{(k+1)} = f (x_{v}^{(k)}, h_{v}^{(k)}, g (\{ h_{u}^{(k)} | u \in N(v) \})) \]
Hierbij:
- \( h_v^{(k)} \) is de toestand van de knoop \( v \) op iteratie \( k \).
- \( x_v^{(k)} \) is de input van de knoop \( v \) op iteratie \( k \).
- \( N(v) \) zijn de naburige knopen van \( v \).

## Gated GNN's
- **Referentie:** [Li et al., 2015]
- De update voor deze GNN's wordt uitgevoerd met een GRU (Gated Recurrent Unit):
\[ h_v^{(k+1)} = GRU (h_v^{