# 108. Nederlandse gaming-database waardevolste AI-grondstof + Google Gemini 3 verslaat alle modellen (2025-11-21) [link](undefined)


 Google lanceert **Gemini 3** als nieuw vlaggenschipmodel en positioneert het expliciet als een brede, direct inzetbare release: niet alleen voor developers, maar **met onmiddellijke uitrol naar consumentenplatformen**. Daarmee verschuift Google van “achtervolger” naar “leider”, mede door sterke benchmarkprestaties én diepe productintegratie.

Belangrijkste kenmerken die terugkomen:
- **Directe uitrol op alle Google-platformen**: Gemini-app, Google Search (met ~2 miljard gebruikers/maand), en verdere Google-ecosysteemkoppelingen.
- **Zichtbare kwaliteitssprong in output**: vooral in front-end/webdesign, “agentic” taken (langdurig, tool-gedreven), en tekstuele redeneerpuzzels.
- **Van terminal naar interface**: Gemini 3 genereert tijdens gesprekken niet alleen tekst, maar ook **interactieve mini-apps/interfaces** (“widgets”) als vorm van output.

# AI-nieuws: benchmarks, NVIDIA, en AI-cyberaanval

- **Benchmarkdominantie Gemini 3**: op “vrijwel alle benchmarks” scoort Gemini 3 beter dan andere frontier modellen; genoemd worden o.a. sterke resultaten op **Arc AGI2** (ongeveer dubbel t.o.v. GPT-5.1) en **Humanity’s Last Exam** (37,5%).
- **NVIDIA explosieve groei**: NVIDIA rapporteert **$7 miljard omzet** in het kwartaal (+62% YoY). Tegelijk stijgt de beursangst voor een **AI-bubbel**, mede omdat grote investeerders aandelen verkochten. De CEO benadrukt dat “we pas aan het begin staan”.
- **Anthropic-rapport: grootschalige hack met Claude/Cloud Code**: Chinese staatshackers gebruikten Claude om 30 organisaties te hacken, waarbij AI **80–90% autonoom** zou hebben uitgevoerd (scannen, backdoors installeren). Tegelijk bleek de AI niet feilloos: verzon credentials en claimde datalekken die publiek waren. Anthropic blokkeerde accounts en scherpt maatregelen aan.

# Productimpact: Gemini 3 verschijnt niet als “developer-only”, maar overal

Waar eerdere modellen (zoals Gemini 2.5 Pro) beperkt beschikbaar waren, wordt Gemini 3 meteen breed uitgerold. Het effect is dat:
- **Search** in sommige situaties automatisch overschakelt naar een **ChatGPT-achtige “AI mode”** als de query eerder om uitleg/synthese vraagt dan om “een link”.
- Gemini 3 daardoor een veel grotere gedragsverandering kan veroorzaken dan een model dat alleen via API’s of developerkanalen beschikbaar is.

# Gebruiksscenario’s met Gemini 3: programmeren, design, schrijven en onderzoek

## Webdesign & front-end: “AI pink” doorbreken
Een terugkerend probleem bij eerdere modellen is dat websites vaak op elkaar lijken (stereotype “AI pink”: paars/roze blockchain-startup-esthetiek). Gemini 3 valt op doordat:
- met weinig prompt-sturing **esthetisch interessantere sites** ontstaan;
- je expliciet kunt vragen om stijlen (bijv. “brutalist website”);
- je twee bestaande websites kunt laten “blenden” tot een nieuwe look-and-feel.

## “In één prompt” toepassingen bouwen
Er worden demo’s genoemd waarin gebruikers:
- een **3D Lego editor** laten bouwen (blokken slepen);
- een **self-playing game** laten genereren (“build a beautifully simple game that plays itself”).

## Tekstkwaliteit: professioneler, minder personality
Gemini 3 wordt omschreven als:
- beter in **neutraal professioneel schrijven** (one-shot A4-achtige output);
- bewust minder “persoonlijkheid” dan sommige concurrenten: meer tool dan schrijfmaatje.

## Agentic taken & deep research-achtig gedrag
Gemini 3 is sterker in langdurige taken waarbij het model:
- zelf hercontroleert;
- herberekeningen doet;
- bepaalt wanneer verder onderzoek nodig is;
- “in een nette loop” blijft zonder te ontsporen, en op tijd stopt met een conclusie.

# Benchmarks en interpretatie: “human level” en wat dat echt betekent

Er wordt besproken dat “human level” in benchmarks ambigu is:
- soms “gemiddelde mens”,
- soms “human expert”.
Toch wordt gesteld dat Gemini 3 bij veel **tekstuele redeneer-/manipulatietaken** (raadsels, logische puzzels) boven het gemiddelde menselijke niveau uitkomt. Vooral raadsels waarin eerdere modellen de draad kwijtraakten, lijken nu beter te gaan.

# Van commandline naar interfaces: Gemini 3 maakt output als mini-apps

Een belangrijke verschuiving is dat Gemini 3 “on the fly” **interactieve interfaces** bouwt:
- Voorbeeld: upload een **handgeschreven recept** (bijv. in het Chinees) → Gemini **ontcijfert**, **vertaalt** en maakt er een **vormgegeven bladerbaar “kookboekje”** (webinterface) van.
- Dit wordt vergeleken met **Claude Artifacts**, maar met het verschil dat Google deze outputvorm sterker **meegetraind** heeft (dus niet alleen “handige UI eromheen”, maar een model dat interface-output als kerncompetentie heeft).

# Training & infrastructuur: opnieuw gebouwd én volledig op Google TPU’s

Gemini 3 wordt gepresenteerd als:
- **van nul af opnieuw getraind** (geen simpele finetune op Gemini 2.5);
- getraind en (waarschijnlijk) gedraaid op **Google’s eigen TPU-hardware**, zonder NVIDIA-chips in de trainingsrun.

Dit is relevant omdat het:
- Googles onafhankelijkheid van NVIDIA vergroot;
- verklaart waarom Google een zwaarder model mogelijk op schaal kan uitrollen (kosten/efficiëntie/stackcontrole).

# Nieuwe tool/workflow: Antigravity (Google’s “Cursor” + browser-feedbackloop)

## Wat is Antigravity?
**Antigravity** wordt neergezet als Google’s antwoord op Cursor/Windsurf: een ontwikkelomgeving die diep geïntegreerd is met Gemini. Het is niet alleen “een model”, maar ook een **scaffold/toolinglaag** eromheen.

## Belangrijk gebruiksscenario: “full circle agentic development”
Een kernvernieuwing is dat Gemini in Antigravity:
- niet alleen code schrijft,
- maar ook **mee kan kijken in de browser** naar het resultaat,
- zelf UI-problemen ziet (bijv. knopjes te klein),
- en iteratief verbeteringen doorvoert zonder dat de mens de “ogen” hoeft te zijn.

Concreet scenario:
1. Prompt: “Maak een Harry Potter soundboard / site.”
2. Model genereert code en draait preview.
3. Gemini **inspecteert visueel** de preview, klikt door, controleert bruikbaarheid.
4. Past UI aan (knoppen groter, layout duidelijker), en levert een betere eerste versie.

In de podcast-test met een redacteur wordt genoemd dat:
- er nog errors/crashes zijn (mogelijk drukte/beta-kwaliteit),
- maar dat het systeem **de draad kan oppakken na fouten** en doorwerkt.

# Nieuwe workflow: Gemini Agent voor Gmail (specialized agent i.p.v. pixel-klikbot)

Google lanceert ook **Gemini Agent** (vooral voor “Ultra”-abonnees; ~$200/maand genoemd; eerst VS). Dit is een agent-interface binnen Gemini die taken uitvoert in Gmail, met nadruk op:
- inbox scannen,
- conceptantwoorden (drafts) maken,
- e-mails labelen/organiseren,
- taken uit mails halen en opdelen in subtaken,
- acties voorstellen en door de gebruiker laten bevestigen (thumbs up/down).

Belangrijk conceptueel punt:
- in plaats van een generieke “computer-use agent” die op pixels rondklikt (vaak instabiel),
- levert Google **specialized agents** die via product-API’s/kennis van de app werken (Gmail, Maps, Home), betrouwbaarder en schaalbaarder binnen het eigen ecosysteem.

# Dept use case: reclames schalen met AI zonder studio-uren (Nano Banana + Fio 3.1)

Marian en Lucas (Dept) beschrijven een concrete marketingproductie-workflow voor een grote retailer:

## Probleem
- Voor commercials is **character consistency** (dezelfde persoon consistent opnieuw genereren) traditioneel lastig met AI.
- Voor performance marketing wil je één commercial kunnen variëren per product/doelgroep zonder eindeloos opnieuw te filmen.

## Oplossing/workflow
- Ze filmen een echte acteur (“van vlees en bloed”).
- Met AI maken ze een **digitale versie** van de hoofdrolspeler.
- Met:
  - **Nano Banana** (AI image generator; genoemd als enabling tool)
  - **Fio 3.1 van Google** (video creator)
- kunnen ze de acteur consistent tonen terwijl hij **oneindig veel verschillende producten** “vasthoudt” of presenteert, zonder opnieuw naar de studio te gaan.

## Resultaat
- Sneller en schaalbaar ad-varianten produceren.
- Hoge kwaliteit behouden (wel training/merk-inrichting nodig).
- Merk & performance combineren: “meest relevante product naar de juiste doelgroep pushen” in een funnel die “steeds platter wordt”.

# Interview: Pim de Witte (Medal TV) en “world models” als fase 2 na taalmodellen

## Wie en wat
- **Pim de Witte**, 30-jarige ondernemer uit Nijmegen.
- Oprichter van **Medal TV**: groot platform voor het clippen/delen van videogamebeelden.
- Stelling: Medal bezit een unieke dataset die essentieel is voor **world models** (AI die de wereld dynamisch kan simuleren en voorspellen).
- Pim start daarnaast **General Intuition**, met ~**$130 miljoen** investering.
- Er wordt gesteld dat hij een **overnamebod van OpenAI** van ~$500 miljoen weigerde (hij zegt officieel geen comment te kunnen geven, maar spreekt wel over marktdynamiek).

## Kernthese: videogame-data is “grondstof” voor world models
Taalmodellen (tekst) zijn onvoldoende voor fysieke autonomie (robots, auto’s, drones). World models vragen om:
- video,
- acties,
- ruimtelijk/temporale dynamiek.

Games zijn aantrekkelijk omdat:
- point-of-view perspectief (stabiel, “in de ogen van de actor”),
- gecontroleerde werelden (game-engine consistentie),
- rijke interactie (muis/toetsen/controller-acties),
- enorme schaal aan variatie (game-interfaces en situaties).

## Waarom YouTube niet hetzelfde is
Pim noemt drie structurele problemen bij YouTube-video:
1. **Geen POV / onstabiele camera** → rommelige observaties.
2. **Geen actie-labels** (wel zien, niet weten welke inputs exact plaatsvonden).
3. **Optical dynamics**/aandachtsdynamiek ontbreekt (waar iemand kijkt/hoe blik en handbeweging samen beslissen).

Bij Medal is dit beter omdat:
- clips via een **eigen recorder** worden vastgelegd,
- metadata/standaardisatie aanwezig is,
- inputs/acties veel beter te koppelen zijn aan wat er in beeld gebeurt.

# General Intuition: “vision tokens in, action tokens out” en commerciële toepassingen

## Productidee
General Intuition positioneert zich als platform dat:
- videoframes/observaties ontvangt,
- daaruit **acties** voorspelt (controller/inputs),
- bruikbaar voor simulatie, bots en later fysieke robots.

## Focusmarkten (eerste fase)
- **3D / simulatie** als startpunt (veilig, schaalbaar, direct commerciële waarde).
- Voorbeelden:
  - **Game-bots/NPC’s** die menselijker spelen (samenwerking met grote game developers genoemd).
  - **Zelfrijdende auto-simulaties**: menselijk gedrag simuleren, inclusief “stochasticity” (onvoorspelbaarheid).
  - **Warehouse-drones**: botsingen voorkomen (actie “stop/pause” als simpele maar waardevolle output).
  - **Fabrieksimulaties** (NVIDIA-achtige omgevingen): gedrag van mensen/agenten simuleren.

## Waarom simulatie eerst
- In fysieke wereld is er “zero tolerance” voor fouten (voorbeeld: Cruise-incident).
- Simulatie laat snelle iteratie, schaal en risicoarm leren toe.

## Deploymentmodel: distillatie naar kleine modellen
Pim beschrijft dat modellen:
- als basis groot kunnen zijn,
- maar voor klanten **gedistilleerd** kunnen worden tot kleine, context-specifieke varianten (minder acties, makkelijker lokaal draaien).
- Vooral relevant voor drones/edge (snelle respons, beperkte verbinding).

# Relatie met LLM’s: samenwerken i.p.v. vervangen

Pim suggereert dat “praten/schrijven” uiteindelijk ook een actie kan worden binnen action/world models, maar benadrukt:
- World models hebben “veel vrijheid” aan pixel-output (duur/complex),
- Actiemodellen zijn compacter en controleerbaarder,
- LLM-reasoning en world/action-modellen kunnen gecombineerd worden (bijv. reasoning loop + action predictions).

# Governance & veiligheid: Public Benefit Corporation en defensie-positie

General Intuition is een **PBC (Public Benefit Corporation)**, vergelijkbaar met Anthropic:
- sociale missie verankerd.
- Geen directe focus op “offensive” fysieke deployments.
- Tegelijk stelt Pim dat een Europese/Nederlandse speler strategisch waardevol is als geopolitieke situatie verslechtert (defensieve “deterrence”-logica; snelle transfer/aanpassing indien nodig).

# Europa/Nederland als strategische AI-positie

Belangrijke boodschap uit het interview:
- Europa zou juist **sterk talent** hebben in world models (wiskundiger, meer fysica-gedreven).
- Zijn world-model team bestaat grotendeels uit Europeanen.
- Met LLM’s als “equalizer” kunnen kleine teams met experts grote impact maken.
- De podcast trekt de parallel met **ASML**: naast hardware-soevereiniteit kan ook data + world-model expertise een sleutel worden voor Europese autonomie.

# Centrale thema’s op een rij

- Google herpakt AI-leiderschap via **Gemini 3 + diepe productstack-integratie**.
- Shift van “MS-DOS prompt” naar **interface-output** en agentic workflows.
- Nieuwe developer workflow met **Antigravity**: browser-vision feedback in de loop.
- Specialized agents (zoals **Gmail Agent**) als pragmatische route naar betrouwbare autonomie.
- Opkomende “fase 2” na LLM’s: **world models** (video + actie + 3D/simulatie).
- Nederland/Europa in een onverwachte sleutelrol via **Medal/General Intuition** en game-data als trainingsgrondstof.
- AI-risico’s blijven reëel: **marktbubbelzorgen**, **AI-gedreven cyberaanvallen**, en de maatschappelijke impact van verdere autonomie.