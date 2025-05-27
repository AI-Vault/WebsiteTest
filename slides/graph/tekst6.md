# Uitleg van de Slide: Recurrerende GNN's

## Inleiding
Deze slide bespreekt de vroegste voorbeelden van Recurrerende Graph Neural Networks (GNN's). Ze zijn gebaseerd op het concept van een recurrent netwerk. Belangrijke processen in deze netwerken zijn de UPDATE en AGGREGATE stappen, die in elke iteratie van message passing hetzelfde zijn.

## Belangrijkste Vergelijkingen

### Basisformule
De basisformule voor de toestand van een knoop \(h^{(k+1)}_v\) na een iteratie wordt weergegeven als:

\[ 
h^{(k+1)}_v = f(x_{v}, h^{(k)}_v, g(\{h^{(k)}_{u} | u \in N(v)\})) 
\]

Hierbij:
- \(x_v\) is de feature vector van de knoop.
- \(h^{(k)}_v\) is de toestand van de knoop in de \(k\)-de iteratie.
- \(N(v)\) is de set van buren van knoop \(v\).

### Gated GNN's
Gated GNN's, geïntroduceerd door Li et al. in 2015, maken gebruik van een Gated Recurrent Unit (GRU):

\[ 
h^{(k+1)}_v = \text{GRU}(h^{(k)}_v, \sum_{u \in N(v)} W^{(k)}_u) 
\]

Hierbij:
- De GRU helpt bij het beheren van informatie door gatingmechanismen.

### Stochastische Steady-state Embedding
In het werk van Dai et al. in 2018 wordt een andere aanpak beschreven:

\[ 
h^{(k+1)}_v = (1-\alpha)h^{(k)}_v + \alpha W^{(k)}_{o} \sigma \left( W_2 x_{v} + \sum_{u \in N(v)} W^{(k)}_{r} [h^{(k)}_u \oplus x_{u}] \right) 
\]

Hierbij:
- \(\alpha\) is een leervoorkeurparameter.
- \(W_2\) en \(W^{(k)}_{r}\) zijn gewichten die tijdens het leren worden geoptimaliseerd.
- De functie \(\sigma\) staat voor een activatiefunctie.

## Samenvatting
Deze slide legt de fundamenten van recurrerende GNN's uit, die gebruik maken van updates en aggregaties in elke iteratie. Twee belangrijke benaderingen zijn de Gated GNN’s en Stochastische Steady-state Embedding, die beide unieke methoden gebruiken om informatie te verwerken binnen grafen.