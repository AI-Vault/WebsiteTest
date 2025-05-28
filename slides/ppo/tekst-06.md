# Uitleg van de Slide: Adv. Actor Critic (A2C)

## Stap 1: Actor
In deze stap wordt de huidige toestand \( S_t \) gebruikt om een actie \( a_t \) te genereren via de Actor, die wordt aangeduid als \( \pi_\theta(s, a) \). De Actor definieert de strategie die het model volgt.

## Stap 2: Critic en Milieu
De Actie \( a_t \) die de Actor heeft gekozen, wordt vervolgens ingevoerd in de Critic, die een geschatte waarde \( \hat{q}(S_t, a_t) \) berekent. Daarna wordt de omgeving (Environm.) geüpdatet, wat resulteert in de nieuwe toestand \( S_{t+1} \).

## Stap 3a: Bijwerken van de Policy
Hier wordt de policy geüpdatet. De verandering in de parameters \( \Delta \theta \) wordt gegeven door:
\[
\Delta \theta = \alpha \nabla_\theta(\log\pi_\theta(s,a))\hat{q}(s, a)
\]
waarbij \( \theta_{\text{new}} = \theta_{\text{old}} + \Delta \theta \). Dit proces maakt gebruik van de Policy Gradient Descent-methode.

### REINFORCE Stap
Hier wordt de formule voor de Reinforce methode weergegeven:
\[
L^{PG}(\theta) = E_t[\log \pi_\theta(a_t|s_t) * \hat{q}_w]
\]
Deze stap zorgt ervoor dat de policy het meest wordt aangepast voor acties die hoge q-waarden (oftewel verwachte beloningen) genereren.

## Samenvatting
De slide beschrijft het proces van het Adv. Actor Critic (A2C) algoritme, dat gebruik maakt van een Actor-Critic structuur om de policy te optimaliseren met behulp van een gradient descent methode en verwachte beloningen.