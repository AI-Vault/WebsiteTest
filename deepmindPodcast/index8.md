# 8. Project Astra: exploring a universal AI assistant with Greg Wayne ([link](https://www.youtube.com/watch?v=ctWfv4WUp2I))
# Algemeen overzicht
Het gesprek gaat over Project Astra, een onderzoeksprototype van Google DeepMind dat de grenzen opzoekt van wat mogelijk is met een universele, agentgerichte AI-assistent. De AI is ontworpen om via verschillende apparaten – zoals smartphones, smart glasses en computers – in real-time met de gebruiker samen te werken door visuele, auditieve en tekstuele input te combineren. In deze aflevering legt Greg Wayne, directeur onderzoek bij DeepMind, samen met presentator Hannah Fry uit hoe Project Astra werkt en welke implicaties het heeft voor de toekomstige interactie tussen mens en AI.

# Belangrijke functies en use cases
Project Astra biedt een reeks functies die verder gaan dan traditionele spraakgestuurde assistenten:
- Realtime multimodale interactie: De AI kan de omgeving zien via de camera, luisteren via de microfoon en reageren met een stem, waardoor het de context van een scène kan interpreteren en vragen proactief kan beantwoorden.
- Geavanceerde geheugenfunctionaliteit: Het systeem bewaart een “in-sessie” geheugen van ongeveer 10 minuten, waarin het visuele en auditieve data opslaat die later samengevat en hergebruikt kan worden. Dit geheugen helpt bij het personaliseren van de interacties en onthoudt bijvoorbeeld voorkeuren zoals het al dan niet lekker vinden van bepaalde etenswaren.
- Proactieve ondersteuning: Naast reactieve vragen kan Project Astra suggesties doen (bijv. herinneringen zoals “vergeet niet om sinaasappelsap te kopen”) en helpen bij praktische taken.
- Ondersteuning voor mensen met beperkingen: Door de mogelijkheid om situaties in de omgeving te interpreteren, kan de AI nuttig zijn voor mensen die bijvoorbeeld slecht ziend of autistisch zijn, door hen te begeleiden in dagelijks gebruik en sociale interacties.
- Taalvaardigheid en onderwijs: Het systeem is meertalig en kan naadloos wisselen tussen talen. Het biedt de mogelijkheid om taal te leren door objecten en omgevingsdetails te benoemen, wat vooral nuttig kan zijn in een vreemde stad of tijdens taallessen.

# Architectuur en technische workflow
Project Astra combineert meerdere geavanceerde componenten:
- Een app die video en audio verzamelt en verzendt naar een server.
- Sensorgebaseerde encoders: Er is een vision encoder voor beeldverwerking en een audio encoder die geluidsinvoer direct verwerkt zonder de omweg via spraak-naar-tekst. Dit vermindert de latency en maakt het mogelijk zeldzamere woorden en diverse accenten beter te herkennen.
- De centrale Gemini taalmodel: Deze AI, die onder de motorkap draait, verwerkt de gecombineerde input van beeld, geluid en context en produceert passende responsen.
- Agent-laag: Deze laag maakt het mogelijk om contextueel relevante informatie op te halen via koppelingen met andere services zoals Google Lens, Google Search en Google Maps. Ook fungeert het als schakel tussen de sensorische invoer en de uitvoering van taken.
- Endpointing en voor-selectieve reactieplanning: Het systeem bepaalt wanneer de gebruiker is gestopt met spreken en anticipeert op een volledige reactie terwijl de gebruiker nog spreekt, om zo de interactiestroom natuurlijk te houden.

# Nieuwe tools en AI features
Het prototype introduceert verschillende nieuwe elementen in de wereld van AI-assistenten:
- Multimodale integratie: In tegenstelling tot eerdere AI’s die voornamelijk spraakgestuurd waren, combineert Project Astra beeld- en geluidsinformatie in één geïntegreerde workflow. Dit maakt het mogelijk om objectherkenning (bijv. boeken of een hersenmodel) en optische analyse van whiteboards uit te voeren.
- Proactieve dialogen en redenering: De AI is in staat om niet alleen te reageren op expliciete verzoeken, maar ook om redeneringen te voeren over wat er in de omgeving gebeurt, zoals het tellen van calorieën op een bord of het herkennen van subtiele visuele details.
- Real-time meertalige interactie: Project Astra kan tussendoor wisselen tussen meerdere talen (Engels, Frans, Russisch, enzovoort) en begrijpt de context waarin deze talen worden gebruikt.
- Verbeterde lage latency: Door de modellen en encoder-systemen fysiek dichtbij elkaar in dezelfde datacentercluster te laten draaien en native audio te verwerken, is de responstijd drastisch verminderd, wat resulteert in een vloeiende en natuurlijke interactie.

# Privacy en ethische overwegingen
Er is aandacht besteed aan de privacy van de gebruiker:
- Gebruikers hebben controle over de opgeslagen data en kunnen eerdere interacties inzien of verwijderen. Het systeem rekonstitueert zijn kennis over de gebruiker telkens wanneer data wordt gewist.
- Veiligheidsfilters en ethische richtlijnen zijn geïntegreerd om ongewenst gedrag of schadelijke content (zoals pornografisch materiaal) te detecteren en te blokkeren.
- Er is nauwe samenwerking met ethici, zoals Iason Gabriel, om ervoor te zorgen dat de AI-assistent op een verantwoorde en mensgerichte wijze wordt ontwikkeld.

# Toekomstige ontwikkelingen
Greg Wayne bespreekt dat de verdere ontwikkeling zich in verschillende richtingen zal uitstrekken:
- Proactieve video-assistentie: Het verder verbeteren van de begeleiding in real-time, bijvoorbeeld voor slechtzienden door hen te waarschuwen voor objecten in hun directe omgeving.
- Full duplex communicatie: De AI zal simultaan kunnen luisteren en spreken, wat een natuurlijkere dialoog mogelijk maakt doordat het kan interacteren met tussentijdse bevestigingen (“uh-huh”) terwijl de gebruiker nog bezig is.
- Verfijning van redenering en geheugen: Meer diepgaande en complexe taken, bijvoorbeeld het automatisch samenvatten van langere conversaties en het redeneren over visuele data (zoals calorie-inhoud op gerechten), zullen verder worden ontwikkeld.
- Verbeterde integratie van externe tools en zoekfuncties: Het systeem zal in staat worden gebracht om bij meer complexe vragen direct andere Google-diensten aan te roepen voor extra informatie en ondersteuning.

Samenvattend markeert Project Astra een significante stap richting een mensachtige, interactief functionerende en meervoudig zintuiglijke AI-assistent die gericht is op zowel praktische dagelijkse hulp als op het verkennen van de fundamenten van kunstmatige intelligentie.