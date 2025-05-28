# Uitleg van de slide: Definiëren van het doellabel y

## Inleiding
De slide bespreekt het proces van het definiëren van het doellabel \( y \) in het kader van een machine learning model voor objectdetectie. Het model is in staat om objecten in een afbeelding te identificeren en te classificeren.

## Doel van de output
Het model moet de volgende informatie opleveren:
1. **\( b_x \)**: De x-coördinaat van de linkerhoek van de bounding box.
2. **\( b_y \)**: De y-coördinaat van de linkerhoek van de bounding box.
3. **\( b_h \)**: De hoogte van de bounding box.
4. **\( b_w \)**: De breedte van de bounding box.
5. **Class label (1-4)**: Een label dat het type object aangeeft:
   - 1 - voetganger
   - 2 - auto
   - 3 - motorfiets
   - 4 - achtergrond

## Voorbeeld
In de slide zie je twee afbeeldingen: de ene toont een auto in de sneeuw (met een bounding box eromheen), en de andere afbeelding toont een sneeuwlandschap zonder objecten die relevant zijn voor classificatie. 

## Structuur van het label \( y \)
De structuur van het label \( y \) wordt geïllustreerd aan de linkerzijde van de slide:

- **\( y \)** wordt gedefinieerd als een vector die bestaat uit:
  - Het waarschijnlijkheidslabel \( p_c \) van het object,
  - De coördinaten \( b_x \), \( b_y \), de hoogte \( b_h \) en de breedte \( b_w \) van de bounding box,
  - Een klasse-indicator \( c_i \) die aangeeft welk type object aanwezig is, waarbij één van de \( c_i \) gelijk is aan 1 (andere zijn 0).

## Conclusie
Door deze structuur te gebruiken, stelt het model niet alleen vast of er een object aanwezig is, maar ook hoeveel ruimte het object inneemt en tot welke categorie het behoort. Dit maakt het mogelijk om zeer accurate objectdetectie te bereiken.