# Uitleg van de Slide

## Titel: Er zijn slechts twee clippings

### Samenvatting
De slide handhaaft dat er in bepaalde machine learning contexten, specifiek in algoritmes zoals Proximal Policy Optimization (PPO), slechts twee clippings zijn. Dit betekent dat de waarde of de gradaties die worden berekend binnen een bepaalde limiet worden behouden om de training te stabiliseren.

### Tabel Uitleg
De tabel geeft verschillende scenario's weer op basis van de waarschijnlijkheid \( p_t(\theta) \) en de actie \( A_t \):

- **Scenario's** worden bepaald door de status van \( p_t(\theta) \).
- **Return Value of min**: hier wordt de minimalem waarde van verschillende opties gekozen afhankelijk van de conditie waaronder \( p_t(\theta) \) valt.
- **Objective is Clipped**: deze kolom laat zien of het doel (de gradient) wordt geclipped of niet.
- **Sign of Objective**: dit geeft aan of het teken van het doel positief of negatief is.
- **Gradient**: toont aan of de gradient van de doelfunctie geldig is onder de gegeven condities.

### Formules
Onder de tabel staan twee belangrijke formules:

1. **Actiewaarde**:
   \[
   A(s,a) = q(s,a) - V(s)
   \]
   Hierbij betekent \( A(s,a) \) de actiewaarde van actie \( a \) in staat \( s \). \( q(s,a) \) is de geschatte waarde van die actie, en \( V(s) \) is de gemiddelde waarde van die staat.

2. **Gemiddelde waarde**:
   \[
   V(s) = \sum [ q(s,a) ]
   \]
   Dit geeft de totale waarde weer van alle acties \( a \) die in staat \( s \) mogelijk zijn.

### Conclusie
Deze slide benadrukt het belang van clippings bij het schatten van waarden en het stabiliseren van de training in reinforcement learning. Door de mogelijkheden binnen bepaalde grenzen te houden, kan men ongewenste oscillaties of divergerende updates voorkomen.