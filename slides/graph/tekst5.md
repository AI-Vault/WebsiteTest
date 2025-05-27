# Uitleg van de Slide: Message Passing Layer

## Concept van Message Passing Layers
- Alle "message passing layers" volgen hetzelfde concept:
  - **k**: Iteratie van message passing.
  - **v**: Node (knop) in een grafiek.

## Formule
- De update van de representatie van een node \( h^{(k+1)}_v \) wordt gegeven door de formule:
  \[
  h^{(k+1)}_v = UPDATE(x_v, h^{(k)}_v, AGGREGATE\left(\{ h^{(k)}_u \mid u \in N(v) \}\right))
  \]
  - Hierin zijn:
    - \( x_v \): De kenmerken van de node.
    - \( h^{(k)}_v \): De huidige representatie van de node.
    - \( N(v) \): De buren van node \( v \).

## Varianten van GNNs
- Varianten van Graph Neural Networks (GNNs) zijn afhankelijk van de keuze van de **UPDATE** en **AGGREGATE** functies:
  - **AGGREGATE** kan zijn:
    - Gemiddelde (Mean)
    - Maximaal (Max)
    - Genormaliseerde som (Normalized Sum)
    - Neuraal netwerk (Neural Network)
  
  - **UPDATE** kan zijn:
    - Gemiddelde (Mean)
    - Maximaal (Max)
    - Neuraal netwerk (Neural Network)
    - Terugkerend neuraal netwerk (Recurrent Neural Network)

Deze structuur maakt het mogelijk om informatie te delen en te leren binnen een grafische representatie, wat van cruciaal belang is voor taken zoals node-classificatie, graf-classificatie en link-prediction.