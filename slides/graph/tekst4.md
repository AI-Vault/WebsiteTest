# Uitleg van de Slide: "Message Passing Layer: Idea"

## Basisconcept

De slide verbeeldt het concept van een "Message Passing" laag binnen een Graph Neural Network (GNN). Deze laag wordt gebruikt om informatie door een grafiek te verspreiden, waardoor knopen (nodes) gegevens ontvangen en versturen van en naar aangrenzende knopen.

## Linkerdeel van de Slide

- **Nodes**: De knopen worden weergegeven als cirkels met verschillende kleuren en nummers erin. Elke node heeft een specifieke set kenmerken.
- **Kenmerken**: Boven elke node staan individuele kenmerkvectoren (\[x1, x2, x3, x4, x5, x6\]) die de kenmerken van die specifieke node representeren.
- **Berichtverzending**: Voor node 1 (blauw) wordt een envelop weergegeven, wat impliceert dat node 1 gegevens of berichten zal ontvangen van zijn aangrenzende knopen (2, 3).

## Rechterdeel van de Slide

- **Verzonden en Ontvangen Informatie**: Na "Message Passing" hebben de knopen nog steeds hun individueel aangewezen kenmerken, maar hun representaties zijn bijgewerkt. Dit bijwerken gebeurt door de kenmerken van naburige knopen te integreren.
- **Illustratie van Node 1**: Node 1 toont nu een veranderde toestand na het doorlopen van het message passing proces