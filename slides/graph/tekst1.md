# Uitleg van de Slide over Graph Reinforcement Learning

## Overzicht

Deze slide behandelt het concept van **Graph Reinforcement Learning**, dat in feite twee hoofdtakken heeft. Elke tak heeft specifieke toepassingen en uitdagingen.

## Deelgebieden

1. **Netwerkrepresentatieleren**
   - **Beschrijving:** Dit onderdeel richt zich op het leren van de representatie van grafen.
   - **Doelstelling:** Ontwikkel een functie (φ) die een graaf (G) omzet in een n-dimensionale ruimte (\( \mathbb{R}^n \)).
   
2. **Adversarial Attacks**
   - **Beschrijving:** Dit gebied betreft het beveiligen van netwerken tegen verstoringen.
   - **Doelstelling:** Maak netwerken robuuster tegen verstoringen in ingevoerde data, zodat de prestaties niet significant dalen als er storingen voorkomen.

3. **Relational Reasoning**
   - **Beschrijving:** Dit richt zich op het analyseren van relaties binnen geordende graafstructuren.
   - **Doelstelling:** Identificeer minimale subgrafen van gerichte acyclische grafen (DAG's) die causaliteit definiëren.

## Toepasbaarheid

- **Op versterkingsleertaken (sequentieel)**
  - **Beschrijving:** Grafen kunnen worden gebruikt in zowel sequentiële leertaken, waarbij de aanpak en methodologie van versterkings