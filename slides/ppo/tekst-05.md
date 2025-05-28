# Uitleg van de Slide over Adv. Actor Critic (A2C)

## Inleiding
Deze slide behandelt het Adv. Actor Critic (A2C) algoritme, een populaire aanpak binnen reinforcement learning. Het A2C-model omvat twee belangrijke componenten: de "Actor" en de "Critic". 

## Stap 1: Actor
- **Indicatoren**: `S_t` en `a_t`
- De actor ontvangt de huidige toestand `S_t` van de omgeving en genereert een actie `a_t` op basis van een beleid \( \pi_{\theta}(s, a) \). Dit beleid bepaalt hoe de agent handelt in een gegeven toestand.

## Stap 2: Critic
- **Indicatoren**: `S_t`, `a_t` en `S_{t+1}`
- De critic ontvangt zowel de toestand `S_t` als de actie `a_t` om een schatting \( \hat{q}_w(S_t, a_t) \) van de waarde van deze toestand-actiekoppeling te verkrijgen.
- Op basis hiervan kan de critic een waarde-effect teruggeven aan de actor, die helpt bij het verbeteren van het beleid.
- De omgeving reageert op de actie van de actor met een nieuwe toestand `S_{t+1}`.

## Samenvatting
In het A2C-algoritme werkt de actor aan het verbeteren van het beleid door acties te kiezen, terwijl de critic de waarde van die acties in de context van de huidige toestand evalueert. Dit dagelijkse proces van interactie en feedback vormt de basis van het leren in reinforcement learning.