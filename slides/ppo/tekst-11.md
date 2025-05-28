# Uitleg van de Slide: Policy Upgrade

## Kernformules

Op de slide zien we verschillende formules die betrekking hebben op het verbeteren van een beleid (policy) in het kader van reinforcement learning. 

1. **Schattingsupdate van het beleid:**
   \[
   \Delta \theta = \alpha \nabla_\theta(\log \pi_\theta(s, a)) \hat{q}_w(s, a)
   \]
   Hierin is \(\Delta \theta\) de verandering in de parameters van het beleid. \(\alpha\) is de leersnelheid, \(\nabla_\theta(\log \pi_\theta(s, a))\) is de gradient van de log van de waarschijnlijkheid van actie \(a\) gegeven staat \(s\). \(\hat{q}_w(s, a)\) is de geschatte waarde van de actie met een bepaalde toestand.

2. **Nieuwe parameters:**
   \[
   \theta_{new} = \theta_{old} + \Delta \theta
   \]
   Hier worden de nieuwe parameters van het beleid berekend door de oude parameters te combineren met de berekende wijziging.

3. **Policy Gradient Theorem:**
   \[
   L^{PG}(\theta) = E_t\left[\frac{\pi_{\theta_{new}}(a_t | s_t)}{\pi_{\theta_{old}}(a_t | s_t)} \hat{q}_w\right]
   \]
   Dit geeft de verwachte waarde van de gradient aan en kan ook worden geschreven als:
   \[
   L^{PG}(\theta) = E_t\left[r_t(\theta) \hat{q}_w\right]
   \]
   Hier is \(r_t(\theta)\) de ratio van de nieuwe en oude beleidsfuncties.

## Ratio van het Beleid

\[
r_t(\theta) = \frac{\pi_{\theta_{new}}(a_t | s_t)}{\pi_{\theta_{old}}(a_t | s_t)}
\]
- Dit laat zien hoe de nieuwe acties van het beleid zich verhouden tot de oude acties.
- Als \(r(t) = 1\), dan verandert het beleid niet; als \(r(t) > 1\), dan is er sprake van een grotere verandering.

### Belang van Beperkingen

Er wordt benadrukt dat we niet willen dat de veranderingen in het beleid te groot zijn. Dit helpt bij het stabiliseren van het leerproces en voorkomt dat het beleid radicale stappen maakt, die mogelijk ongunstig zijn voor de prestaties.