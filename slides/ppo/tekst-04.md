# Uitleg van de Slide: Advantage Actor Critic (A2C)

## Algemeen Overzicht
De slide legt het concept van de Advantage Actor Critic (A2C) uit, een methode binnen reinforcement learning die gebruikmaakt van twee neurale netwerken: de Actor en de Critic.

### Actor
- **Functie**: De Actor neemt beslissingen in een bepaalde toestand (state).
- **Notatie**: 
  - π(s, a) = kans dat in toestand s actie a wordt gekozen.
  - Hierin vertegenwoordigen de gewichten θ de parameters van het model.

### Critic
- **Functie**: De Critic leert de Actor hoe goed zijn beslissingen waren.
- **Notatie**: 
  - Q̂(S_t, a_t) = Q-waarde (verwachte reward) bij actie a_t in toestand S_t.
  - Hierin zijn de gewichten w de parameters van dit model.

### Voordelen
- Deze aanpak zorgt ervoor dat het beleid (policy) niet te snel verandert na het maken van slechte keuzes. Het helpt om de stabiliteit van de leermethode te bevorderen.

## Samenvatting
De Advantage Actor Critic (A2C)-methode combineert de beslissingscapaciteit van de Actor en de evaluatiecapaciteit van de Critic, wat leidt tot efficiënter leren en betere prestaties in reinforcement learning scenario's.