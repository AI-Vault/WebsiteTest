# Proximal Policy Optimization (PPO)

## Algemene Idee:
- Bij het zoeken naar een optimaal beleid ben je een maximum aan het zoeken.
- Je wilt dus naar de top.
- En daarbij moet je niet te grote stappen nemen.
- Want wat gebeurt er anders?
- PPO zorgt voor handrails.

### Uitleg
Proximal Policy Optimization (PPO) is een populaire algoritme in reinforcement learning dat zich richt op het optimaliseren van beslissingsstrategieën (policies). De kernconcepten die hier worden toegelicht, zijn:

1. **Zoeken naar een Optimaal Beleid**: In machine learning probeer je een beleid te vinden dat de beste beslissingen neemt in een gegeven omgeving. Dit beleid moet geoptimaliseerd worden voor maximale prestaties.

2. **Naar de Top**: Hierbij moet je de best mogelijke uitkomst (bijvoorbeeld de hoogste beloning) bereiken, vergelijkbaar met het beklimmen van een berg.

3. **Grote Stappen Vermijden**: Het nemen van te grote stappen in het aanpassingsproces kan leiden tot instabiliteit en slechte prestaties. De algoritme bevordert kleine, beheersbare aanpassingen.

4. **Handrails**: PPO implementeert beperkingen (handrails) op de manier waarop beleidsupdates worden uitgevoerd. Dit zorgt ervoor dat zelfs als het beleid niet perfect is, het binnen veilige grenzen blijft en niet te veel afwijkt van wat al goed werkt. 

Deze aanpak maakt PPO effectief en robuust in het trainen van agenten binnen complexe omgevingen.