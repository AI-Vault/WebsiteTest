# Uitleg van de Slide: Recurrent Graph Neural Networks

## Inleiding

De slide bespreekt vroege voorbeelden van recurrente Graph Neural Networks (GNNs). Deze netwerken zijn gebaseerd op het idee van een recurrent netwerk, waarbij de **UPDATE** en **AGGREGATE** stappen constant blijven voor elke iteratie van message passing.

## Formule voor Update van Nodes

1. **Algemene Update Regel**:
   - De update van de node-representatie \( h_v^{(k+1)} \) wordt bepaald door een functie \( f \).
   - Invoer voor \( f \) bestaat uit:
     - \( x_v \): Oorspronkelijke kenmerken van de node \( v \).
     - \( h_v^{(k)} \): Huidige staat van node \( v \).
     - \( g \): Aggregatiefunctie die informatie verzamelt van de naburige nodes \( u \in \mathcal{N}(v) \).

## Specifieke Implementaties

1. **Gated GNNs (Li et al., 2015)**:
   - Gebruikt een Gated Recurrent Unit (GRU) om de update te berekenen:
   \[
   h_v^{(k+1)} = \text{GRU} \left( h_v^{(k)}, \sum_{u \in \mathcal{N}(v)} W \, h_u^{