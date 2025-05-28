# Uitleg van de Slide: Policy Upgrade Beperken (q Negatief)

Op deze slide wordt besproken hoe we de policy upgrade kunnen beperken wanneer het рисiki heeft dat q negatief is. Hieronder volgen de belangrijkste onderdelen van de slide:

## Formule voor Beperking

- **Formule**: 
  $$ r_t(\theta) = \frac{\pi_{\theta\text{new}}(a_t | s_t)}{\pi_{\theta\text{old}}(a_t | s_t)} < 1 $$
  
  Hieruit blijkt dat als de verhouding van de nieuwe policy ten opzichte van de oude policy kleiner is dan 1, dan wordt de kans op actie $ \pi_{\theta}(a_t | s_t) $ groter.

## Doel van de Beperkingen

- De slide benadrukt dat we de veranderingen in de policy willen beperken om te voorkomen dat de aanpassing te groot wordt. Dit is cruciaal voor de stabiliteit van het leersysteem.

## Afsnijding van Veranderingen

- We willen wijzigingen in de policy beperken tot $ 1 - \epsilon $, maar alleen wanneer $ q < 0 $ is. Dit betekent dat als de schatting van de waarde (q) negatief is, we de policy-aanpassing op een gecontroleerde manier willen beperken.

## Grafische Representatie

- De grafiek toont een visuele weergave van de relatie tussen de ratio $ r_t(\theta) $ en $ \hat{q}_w $ (de geschatte waarde).
- De zwarte lijn vertegenwoordigt de beperking, waarbij waarden onder $ L_{\text{CLIP}} $ worden vastgezet.
- De rode stip toont de plaats waar de aanpassing wordt afgekapt, waardoor grote schommelingen in de policy worden voorkomen.

## Loss Functies

- **Loss functie**:
  - $$ L^{PG}(\theta) = E_t [r_t(\theta) \hat{q}_w] $$
  - $$ L^{CLIP}(\theta) = \hat{E}_t [\min(r_t(\theta), 1 - \epsilon) \hat{q}_w] $$
  
  Deze functies berekenen de waarden die we proberen te optimaliseren tijdens het trainen van het model.

## Conclusie

De slide legt uit hoe het belangrijk is om de policy upgrades te beperken, vooral wanneer er risico's zijn van negatieve q-waarden. Dit helpt bij het waarborgen van de stabiliteit en betrouwbaarheid van het algoritme dat leert van zijn omgeving.