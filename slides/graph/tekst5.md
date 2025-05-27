# Uitleg van de Slide: Message Passing Layer

## Message Passing Laag

- Alle message passing lagen volgen hetzelfde concept (waarbij \( k \) de iteratie van message passing is en \( v \) een knoop).
  
- De update formule voor een knoop \( v \) is als volgt gedefinieerd:
  
\[ 
h_v^{(k+1)} = \text{UPDATE}\left(x_v, h_v^{(k)}, \text{AGGREGATE}\left(\{h_u^{(k)} \,|\, u \in \mathcal{N}(v)\}\right)\right) 
\]

### Uitleg van de Formule

- **\( h_v^{(k+1)} \):** Dit is de geüpdatete representatie van knoop \( v \) na \( k+1 \) iteraties.
- **UPDATE:** Een functie die de knoop- en buurtrepresentaties combineert tot een nieuwe representatie.
- **AGGREGATE:** Een functie die de representaties van de aangrenzende knopen (\( \mathcal{N}(v) \)) samenvoegt.
  
### Varianten van Graaf Neurale Netwerken (GNNs)

- De verschillende varianten van GNNs hangen af van de keuze van de functies **UPDATE** en **AGGREGATE**. Bijvoorbeeld:
  - **AGGREGATE:**