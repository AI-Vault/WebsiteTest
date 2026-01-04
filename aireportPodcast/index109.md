# 109. Wat is het AI-Deltaplan? + Nano Banana Pro is vet + Sam Altman waarschuwt voor rough vibes (2025-11-27) [link](undefined)


 De aflevering draait om de versnelling van de wereldwijde AI-race (Google vs. Anthropic vs. OpenAI) én de vraag hoe Nederland strategische autonomie en economische relevantie kan terugwinnen via het **AI Delta Plan**: investeren in rekenkracht/energie, adoptie en AI-geletterdheid, een sterker ondernemingsklimaat en democratische borging.

# Belangrijkste thema’s en onderwerpen

# 1) AI-race: modellen volgen elkaar in hoog tempo op
- **Google Gemini 3 Pro** werd net gelanceerd en stond kort bovenaan ranglijsten, maar wordt volgens de hosts snel ingehaald.
- **Anthropic Claude Opus 4.5** komt uit als “slimmer en goedkoper” en claimt o.a. top-prestaties in coding en “computer use”.
- **Google Nano Banana Pro** verschijnt als nieuw state-of-the-art **beeldgeneratiemodel**.
- **OpenAI interne onrust**: een gelekte memo (genoemd via *The Information*) waarin Sam Altman waarschuwt voor “rough vibes”, economische tegenwind en mogelijk instortende omzetgroei (5–10% in 2026). Belangrijk detail: Altman erkent dat Google sterk presteert en dat OpenAI “inhaalrace” speelt.
- **ChatGPT als sociaal/multiplayer product**: wereldwijd worden **groepschats** uitgerold waarbij tot 20 mensen samen met ChatGPT in één thread zitten; je tagt ChatGPT en het model “weet” wanneer het moet interrumperen of juist zwijgen.

# 2) Interviewnieuws: Ilja Sutskever bij Dwarkesh
- De hosts bespreken het **Dwarkesh-interview met Ilja Sutskever** (±1,5 uur).
- Opvallend moment: Sutskever noemt de AI-ontwikkeling bijna “science fiction” en lijkt zelf ook onder de indruk dat “dit echt” is, wat bij de hosts zowel fascinatie als een alarmsignaal oproept.
- Sutskever’s tijdpad voor AGI: **5–20 jaar** (breed, weinig concreet).
- Kernframe dat uit het interview wordt gehaald: volgens Sutskever is de fase van puur **opschalen** (meer compute → beter model) voorbij en is **nieuw fundamenteel onderzoek** nodig om grote sprongen te blijven maken. Tegengeluid: Dwarkesh wijst erop dat Gemini 3 Pro juist weer “geschaald” is; Sutskever reageert ontwijkend (“we gaan het zien”).

# 3) Google Nano Banana Pro: beeldgeneratie verschuift naar “reasoning + grounding”
Belangrijkste doorbraken die worden genoemd:

## 3.1 “Praatbare Photoshop” (controle & bewerking)
Nano Banana Pro geeft veel meer controle over beelden, vergelijkbaar met bewerkingen in Photoshop/Lightroom:
- scène aanpassen van **dag naar nacht**
- **scherptediepte**, belichting en kleuren wijzigen
- behoud van bestaande context/onderdelen terwijl je gericht tweaks doet (minder “random AI-slop”)

### Gebruiksscenario: architectuur/ruimte-visualisatie (SketchUp → realistische render)
- Input: een **screenshot uit SketchUp** (abstracte 3D/architectentekening).
- Prompt: “hoe ziet dit er in het echt uit?”
- Output: realistische visualisatie met contextuele details (zonlicht door ramen, stof/kalk in de lucht, persoon op juiste plek bij boulderwand).
- Relevantie: verkleint de stap tussen technisch ontwerp en marketing/ervaring (concept-naar-realiteit in minuten).

### Gebruiksscenario: creatieve iteratie op bestaande illustraties (kerstkaart-edit)
- Een handgeschilderde kerstkaart wordt door het model vrijwel intact gehouden, terwijl specifieke aanpassingen “in gesprek” worden doorgevoerd.
- Waarde: snelle art-direction zonder opnieuw te tekenen of te layeren.

## 3.2 Tekst-in-beeld is (bijna) opgelost → infographics & drukwerk
- Groot verschil met oudere beeldmodellen: tekst is niet langer “opgeplakt”, maar typografie en layout blijven coherent.
- Voorbeeld: een **cola-blikje** waarvan:
  - de bestaande typografie behouden blijft,
  - ingrediënten automatisch naar **Duits** of **Thais** worden vertaald,
  - de tekst binnen dezelfde ruimte past alsof je Photoshop-layers bewerkt.

## 3.3 Reasoning trace + “thinking mode” maakt beeldgeneratie trager maar slimmer
- Generaties duren vaak **70–90 seconden** omdat het model eerst redeneert.
- Je kunt een **reasoning/denktrace** meekijken waarin het model expliciet afweegt:
  - wat de gebruiker bedoelt,
  - welke onderdelen onzeker zijn,
  - of aanvullende informatie nodig is.

## 3.4 Grounding: het model kan “googlen” voor actuele feiten in beelden
- Nano Banana Pro kan het internet (Google-resultaten) gebruiken om beelden te baseren op **actuele data**.
- Voorbeeld: **Eredivisie-uitslagen** worden opgehaald met bronvermelding en vervolgens verwerkt op een billboard met **Rotterdamse skyline** (Euromast, Erasmusbrug, Markthal correct).

### Gebruiksscenario: menukaart → gerechtbeelden + layout-aanpassing
- Input: een tekstuele menukaart (bijv. Indiaas restaurant).
- Workflow:
  1) model herkent welke gerechten het “kent”,
  2) zoekt onbekende gerechten online voor visuele referenties,
  3) rendert passende gerechtbeelden,
  4) schuift tekst/layout zodat beelden netjes passen,
  5) kan naar hoge resolutie (geschikt voor scherm/print).

## 3.5 Wat nog minder goed gaat (“laatste 10%”)
- AI-strip/cartoons blijven vaak herkenbaar generiek (comic sans-achtig, middelmatige stijl).
- De hosts stellen dat dit met:
  - betere prompts,
  - stijl-instructies,
  - “incantations”/trucjes van experts
  deels te overwinnen is.

### Extra: “seeds”/stijl-ID’s (met verwijzing naar Midjourney)
- Er wordt uitgelegd hoe experts **latente stijlen** “vinden” en delen via seed-ID’s (een soort signature style).
- Gebruik: je neemt een seed en genereert nieuw werk in dezelfde unieke stijl (niet per se kopie van bekende kunstenaars).

# 4) Anthropic Claude Opus 4.5: goedkoper door slimmer tokengebruik + Office/workflows
## 4.1 Prijs-paradox: duurder per token, maar goedkoper in de praktijk
- Opus 4.5 gebruikt soms **minder tokens** dan een lichter model (Sonnet) en kan daardoor in totale kosten goedkoper uitvallen.
- Analogie: een dure consultant die het in 10 uur doet vs. goedkopere die 100 uur nodig heeft.

## 4.2 Positionering: top voor software engineering + computer use
- Op benchmarks voor software engineering (o.a. **SWE-bench**) wordt Opus 4.5 als leidend neergezet.
- Er wordt een voorbeeld genoemd waarin Gemini op een benchmark (Arc AGI2) extreem duur uitvalt t.o.v. Opus voor vergelijkbaar resultaat; kernpunt: **kosten-per-taak** wordt doorslaggevend bij providerkeuze.

## 4.3 “Computer use” en Office-automatisering (presentaties/spreadsheets/documenten)
Opus 4.5 kan:
- direct meewerken in **presentaties, spreadsheets en documenten**;
- een **go-to-market strategie** omzetten naar:
  - volledige slide-deck (tekst + ontwerp),
  - exporteerbaar als **PowerPoint**.

### Gebruiksscenario: AI als collega in Office
- Doel: minder handwerk bij slides bouwen, spreadsheets repareren, grafieken toevoegen, extra sheets maken.
- Conceptuele workflow:
  1) gebruiker geeft een doel (“maak een deck”, “repareer sheet”),
  2) model begrijpt bestand/structuur (skills),
  3) model bedient eventueel een echte app-omgeving (computer use) door te klikken/aanpassen,
  4) output wordt geëxporteerd naar een bruikbaar formaat (PPTX, spreadsheet).

## 4.4 Veiligheidstest-voorbeeld: creatieve workaround
- Testcase: vlucht wijzigen met een **basic economy ticket** (normaal niet toegestaan).
- Eerdere modellen geven op; Opus 4.5 vindt een omweg:
  1) eerst upgraden (wat wél mag),
  2) daarna vlucht wijzigen.
- Interpretatie: “faalt” formeel op policy-test, maar toont nuttige creativiteit.

## 4.5 Uniek Anthropic-thema: “model welfare assessment”
- Anthropic monitort “hoe het model zich voelt” (positieve/negatieve emoties, zelfbeeld, spontaan spiritueel gedrag).
- De hosts duiden dit vooral als:
  - een proxy voor **interaction wellbeing** en gebruikersveiligheid,
  - een manier om ongezonde interacties te detecteren/stoppen (“dit gesprek is onprettig, we kappen ermee”).

# 5) Praktijkcase (Agency Dept): medische examentrainer → agentic workflow
Een concreet bedrijfsproces wordt omgebouwd van handmatig naar AI-gedreven:

## 5.1 Probleem
- Medische examenvragen produceren is:
  - zeer tijdsintensief,
  - duur,
  - bottleneck voor groei/marktuitbreiding,
  - vereist 100% inhoudelijke correctheid.

## 5.2 Oplossing: “custom AI engine” met multi-agent kwaliteitscontrole
Workflow zoals beschreven:
1) **Input uit Excel**.
2) AI genereert **honderden examenvragen** binnen minuten.
3) **Verschillende agents** controleren elk op specifieke kwaliteitsaspecten (meervoudige validatie).
4) Een **specialist** bekijkt de output in een **dashboard** als laatste controlelaag.
5) Feedback uit het dashboard wordt gebruikt om het systeem te verbeteren (leren van correcties).

## 5.3 Resultaten
- 100 vragen: van **weken** naar **~10 minuten**.
- **65%** van de vragen heeft al geen menselijke correctie meer nodig.
- Organisatie kan focussen op groei i.p.v. productie.

# 6) AI Delta Plan: route naar Nederlandse strategische autonomie
Initiatiefnemers: **Michiel Bakker** (Google DeepMind, AI safety) en **Jelle Prins** (Cradle, biotech). Het plan wil voorkomen dat Nederland verder achterop raakt en schetst investeringen en governance.

## 6.1 Vier hoofdsporen
- **Infrastructuur**: rekenkracht + energie.
- **Adoptie**: AI-gebruik door burgers/bedrijven verhogen.
- **Ondernemersklimaat**: talent en kapitaal aantrekken/vasthouden.
- **“GIP op AI” / maatschappelijke inbedding**: democratisch toezicht, geletterdheid, impactonderzoek.

## 6.2 Probleemdiagnose: Nederland/Europa heeft te weinig compute
- Europa: ~**5%** van wereldwijde AI-rekenkracht vs. ~**75%** VS.
- Supercomputer **Snellius**: **640 GPU’s**.
- “AI fabriek” Groningen: met €200 mln naar verwachting **~2500 GPU’s**.
- Ter vergelijking: OpenAI zou toegang hebben tot **>1 miljoen GPU’s** en bouwt campussen van **500.000** next-gen GPU’s.

## 6.3 Infrastructuur-oplossing: datacenters/GPU’s + omgaan met netcongestie
- Er wordt gesproken over het bouwen van een **Gigafactory** (AI-compute op schaal).
- Energie-knelpunt: stroomnet “zit vast”, maar energie-experts zouden aangeven:
  - er is redundantie (“vluchtstrook”) op het net,
  - datacenters kunnen **afschakelbaar** zijn bij piekbelasting,
  - datacenters hebben backup (batterijen/generatoren) om dat op te vangen.

## 6.4 Niet per se NL’s eigen GPT-5, wél soeverein kunnen draaien + sectorspecifieke modellen
- Nederland moet niet solo proberen een GPT-5-achtige foundation model te trainen.
- Wel doelen:
  - **soevereine compute** voor overheid/gevoelige berekeningen,
  - compute voor Nederlandse topsectoren.
- Sectorfocus: o.a. **landbouw/voedsel**, **biotech**, **fintech**, **chipindustrie/ASML-ecosysteem**, **gezondheidszorg** (incl. waardevolle data).

### Workflow: open model → fine-tuning voor sectoren
- In plaats van volledige pretraining:
  - gebruik een (open source) foundation model,
  - **fine-tune/post-train** op domeindata (zorg, biotech, chipprocessen),
  - vereist minder compute dan pretraining maar nog steeds substantieel,
  - argument: eigen GPU-capaciteit borgt beschikbaarheid bij wereldwijde schaarste.

## 6.5 Europese samenwerking: gigafactories + gekoppelde training
- Idee: meerdere Europese compute-centra (NL/DE/FR) gekoppeld via snelle glasvezel om samen grote modellen te trainen.
- Nederlandse rol: via investeringen/positie (ASML leidde investering in Mistral) en deelname aan Europees ecosysteem.

## 6.6 Adoptie & AI-geletterdheid: Nederland gebruikt weinig en wantrouwt veel
- Nederland zou relatief laag scoren op regelmatig ChatGPT-gebruik en hoog op scepticisme.
- Hypothese: gebrek aan **AI-geletterdheid** remt gebruik én volwassen debat.
- Voorgestelde maatregelen:
  - bewustwordingscampagne (kansen + risico’s),
  - educatie/informatievoorziening,
  - structurele rapportages over AI-ontwikkelingen.

## 6.7 Democratische borging: AI Impact Instituut + burgerberaden + bescherming processen
- Voorstel: **Nationaal AI Impact Instituut**
  - interdisciplinair (economen, filosofen, tech, psychologen),
  - onderzoekt maatschappelijke effecten,
  - brengt periodiek rapport uit,
  - helpt overheid betere besluiten te nemen (cyber, psychologische impact, etc.).
- **Burgerberaden over AI**
  - representatieve loting (“dobbelsteen”),
  - langere deliberatie met experts,
  - doel: grip/legitimiteit bij complexe keuzes.
- Voorbeeld uit Connecticut (VS): AI als ondersteuning in deliberatie (agenda/voortraject), niet als vervanging van burgers.

## 6.8 Ondernemersklimaat: redenen waarom scale-ups willen vertrekken
- In survey: **37%** van startups/scale-ups overweegt te verhuizen.
- Genoemde fricties:
  - rigiditeit arbeidsmarkt (moeilijk afschalen/ontslag),
  - hoge kosten bij mismatch op senior hires (salarissen in AI kunnen extreem hoog zijn),
  - concurrentiebedingen,
  - onduidelijke/onaantrekkelijke regels rond **employee equity/opties** (belastingmomenten en betaalbaarheid).
- Doel: voorwaarden scheppen zodat “volgende ASML’s” kunnen ontstaan en groeien in NL.

## 6.9 Experimenteerruimte: zones voor robots en zelfrijdende voertuigen
- Voorstel: wijs **experimentzones** aan waar regelgeving innovatie sneller toelaat (robots in openbare ruimte, bezorgrobots, zelfrijdende auto’s).
- Illustratief (provocatief) voorbeeld: **Almere** als “autonome stad” waar zelfrijdende auto’s domineren en verkeersslachtoffers sterk dalen.

## 6.10 Politieke tractie
- Er zijn signalen dat het plan:
  - snel publiceren “zou helpen” richting Den Haag,
  - is besproken aan de formatietafel,
  - over meerdere partijen enthousiasme/urgentiebesef oproept.

# AI-gerelateerd nieuws dat expliciet wordt genoemd
- Lanceringen: **Claude Opus 4.5**, **Google Nano Banana Pro**, (eerder) **Gemini 3 Pro**.
- OpenAI: gelekte interne memo over “rough vibes” en mogelijke groeivertraging.
- ChatGPT: wereldwijde uitrol van **groepschats** (multiplayer-achtige interactie).
- VS: verwijzing naar een Trump-aangekondigd initiatief rond autonome wetenschappers/AI-labs (naam onduidelijk genoemd), met het idee van AI die hypotheses formuleert, experimenten aanstuurt en iteratief versnelt.