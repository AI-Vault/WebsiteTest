# Definitie van de Doel Label y

## Klassignaamgeving
In de slide worden vier klassen geïntroduceerd die moeten worden geclassificeerd:

1. **Pedestrian**
2. **Auto**
3. **Motorfiets**
4. **Achtergrond**

### Uitvoervereisten
Bij het trainen van een model dat deze objecten herkent, moeten de volgende waarden worden output:

- \(b_x\): De x-coördinaat van de bounding box
- \(b_y\): De y-coördinaat van de bounding box
- \(b_h\): De hoogte van de bounding box
- \(b_w\): De breedte van de bounding box
- **Klasse label**: Een waarde van 1 tot 4 die overeenkomt met een van de hierboven genoemde klassen.

## Kostenfunctie
De kostenfunctie \(L(\hat{y}, y)\) wordt gedefinieerd als:

\[
L(\hat{y}, y) =
\begin{cases} 
(\hat{y}_i - y_i)^2 + (\hat{y}_j - y_j)^2 + \ldots + (\hat{y}_n - y_n)^2 & \text{als } y_i = 1 \\ 
(\hat{y}_i - y_i)^2 & \text{als } y_i = 0 
\end{cases}
\]

Hierbij staat \( \hat{y} \) voor de voorspelling van het model en \( y \) voor het werkelijke label.

### Interpretatie van de Output
- Als er een object (bijvoorbeeld een auto) aanwezig is (\(y_i = 1\)), worden de fouten voor alle voorspellingen van dat object berekend.
- Als er geen object aanwezig is (\(y_i = 0\)), wordt alleen de relevante fout voor die situatie berekend.

## Voorbeeld
In het voorbeeld op de afbeelding zijn er twee verschillende beelden. In het linkerbeeld is er een auto aanwezig (en de overeenkomstige bounding box is gemarkeerd), terwijl in het rechterbeeld de achtergrond wordt weergegeven zonder herkenbare objecten. 

Hierbij is:

- \(x\): De input afbeelding.
- \(y\): De output labels, waarbij de specifieke waarden voor de bounding box en het klasse label worden weergegeven:

\[
y = 
\begin{bmatrix}
1 \\
b_x \\
b_y \\
b_h \\
b_w \\
c_1 \\
c_2 \\
c_3
\end{bmatrix}
\]

Met \(c_1, c_2, c_3\) die de kans op de drie verschillende objecten representeren.

In het geval dat er geen object is ("don't care"), wordt dit ook correct aangegeven in de output.