# 111. Zeskoppige start-up kraakt 'onmogelijke' AI-test + Sam Altman haalt GPT-5.2 naar voren + MCP gaat... (2025-12-10) [link](undefined)


 De aflevering draait om een opvallende versnelling in AI-capaciteiten zoals gemeten door een zware “general intelligence”-benchmark (Arc AGI 2). De kern: een kleine start-up (Poetic, 6 personen) breekt door de 50%-grens zonder een eigen foundation model te trainen, maar door een slim “softwarepak” (scaffolding) om een bestaand model (Gemini 3 Pro) heen te bouwen. Dit voedt de bredere discussie: komt vooruitgang vooral uit grotere modellen, of juist uit betere workflows, integraties en “test-time” (inference) architecturen?

# Belangrijkste thema’s en onderwerpen
# AI in cultuur en marketing: kerstcommercials als strijdtoneel
- Reclamebureaus delen massaal AI-gegenereerde kerstcommercials (o.a. Coca-Cola internationaal, McDonald’s NL).
- LinkedIn-communicatie eromheen is dubbel: trots op innovatie, maar met veel disclaimers (“experimenteren”, “innoveren”) vanwege voorspelbare kritiek (authenticiteit, ‘zielloos’, energieverbruik, etc.).
- Tegentrend/statement: een kleiner bureau pronkt juist met een volledig handgemaakte stop-motion/klei-commercial (Wallace & Gromit-stijl). De handmatige productiewijze wordt zelf een signaal/waardepropositie.
- Meta-content als “bewijs van echtheid” groeit: making-of video’s (zelfs “making-of van de making-of”) worden belangrijker naarmate AI-content lastiger te onderscheiden is van handwerk.
- Speculatie: als AI-output straks niet meer te herkennen is, wordt “handgemaakt” vooral nog waardevol via het verhaal eromheen (making-of, transparantie, ambacht).

# OpenAI: focus terug naar modelupdates, reclame uit ChatGPT
- Gerucht: GPT-5.2 verschijnt eerder dan gepland (mogelijk al deze week), als tussenrelease.
- OpenAI testte advertenties in ChatGPT; betaalde gebruikers klaagden, functie is uitgezet.
- In het verhaal: een interne “code rood” (concurrentiestrijd met Google) leidt tot herprioritering: eerst kernkwaliteit en modelprogressie, advertentieplannen later.

# Integratie wint van “beste model”: AI schuift dieper in werksoftware
- De aflevering benadrukt dat de competitie verschuift van “welk model is het best?” naar “wie integreert het diepst in bestaande workflows?” (Slack, IDE’s, bedrijfsapps).

# Cloud Code naar Slack: vibe coding in de werkchat
- Tool/feature: “Cloud Code” (vibe coding tool op basis van Anthropic’s Claude-model) komt naar Slack.
- Gebruiksscenario:
  - In een Slack-gesprek met collega’s kun je Claude taggen (zoals een collega) met een verzoek als “debug dit” of “help dit stuk code verbeteren”.
  - De AI pakt de taak op vanuit de chatcontext.
- Relevantie: AI wordt een “collega in de werkchat”, niet een losse website. Dit sluit aan bij bestaande integraties (Cursor, GitHub Copilot + Slack).
- Implicatie: adoptie wordt bepaald door frictieloos gebruik op plekken waar werk al gebeurt (Slack), niet alleen door benchmarkwinsten.

# Grote doorbraak in Arc AGI 2: Poetic over 50% met Gemini + scaffolding
- Arc AGI 2 wordt neergezet als een “lakmoesproef” voor generalisatie: nieuwe, onbekende puzzels oplossen zonder te leunen op eerder geziene voorbeelden.
- Context:
  - Arc AGI 1 werd “gekraakt” door OpenAI’s redeneermodel (O1) met ~75–85%.
  - Arc AGI 2 zette de sector terug op aarde: mensen gemiddeld ~60%, experts 100%, topmodellen (destijds o.a. O3-high) rond ~4% en zeer duur (~$200 per taak).
  - 6 maanden geleden zaten topmodellen nog <5%.
- Nieuws:
  - Poetic (6 personen, ex-DeepMind/Google-profielen) is als eerste door 50% heen op Arc AGI 2.
  - Ze trainen geen eigen model: ze gebruiken Google’s Gemini 3 Pro en bouwen er “slimme software” omheen.
  - Resultaat: beter dan Google’s eigen topvariant op die test, tegen ~halve kosten; genoemd wordt ~$30 per opgave.

# Wat Poetic technisch doet: “Superman pak / exoskeleton / scaffolding”
- Kernidee: vooruitgang komt niet alleen van pretraining (train compute), maar ook van “test-time compute” (inference compute) + software-architectuur rond het model.
- Het “scaffold” werkt model-agnostisch (zij testen ook andere modellen: GPT, Claude, Gemini 2.5 destijds), waardoor het niet een Gemini-specifiek trucje is maar een generieke versterker.
- Belangrijkste workflow/AI-architectuur elementen (zoals beschreven):
  - Sterke startprompt: een zorgvuldig ontworpen “puzzeloplos”-prompt.
  - Leren tijdens gebruik (“recurring learning”):
    - In plaats van per puzzel een nieuw gesprek met “vergeten” context, worden inzichten/fouten expliciet vastgelegd en hergebruikt in volgende pogingen.
    - Falen wordt informatie: de prompt/flow is zo ingericht dat het model niet alleen “fout” hoort, maar ook systematisch analyseert wat er misging.
  - Meerdere parallelle kopieën/agents:
    - Meerdere Gemini-instanties werken parallel aan dezelfde taak, genereren hypotheses en delen inzichten.
  - Consensus/democratische selectie:
    - Outputs/ideeën worden vergeleken; er ontstaat een soort “jury”/stemronde om de beste hypothese/route te kiezen.
  - Slim budgetteren van pogingen:
    - Arc AGI 2 geeft (volgens het gesprek) beperkte pogingen; de strategie lijkt op: eerste poging verkennen/diagnosticeren, tweede poging optimaliseren op basis van geleerde signalen.
- Conceptuele implicatie (separation of concerns):
  - “Wat hoort in het basismodel?” versus “wat hoort in de runtime-softwarelaag?”
  - Mogelijk ontstaat een stabiele AI-architectuur waarbij foundation models componenten zijn (zoals CPU’s), en het echte “intelligente gedrag” uit lagen eromheen komt (scaffolds, agents, geheugen, planners).

# Nieuwe benchmarks op komst: van statische puzzels naar interactieve omgevingen
- Verwachting: een volgende Arc-variant verschuift naar interactieve game-achtige benchmarks:
  - Waarnemen-beslissen-handelen over meerdere stappen
  - Exploratie, planning, geheugen, doelen begrijpen
  - De taak verandert terwijl je ermee bezig bent (niet meer “uitprintbaar”)
- Reden: zodra een benchmark wordt ingehaald (door betere modellen of betere scaffolds), moet hij evolueren om generalisatie en adaptief leren beter te testen.

# Debat over “95% kenniswerk overnemen” en ensemble-AI
- Sceptici (zoals Gary Marcus wordt genoemd) stellen: taalmodellen zijn vooral statistische “bluffers” en schalen niet naar echte algemene intelligentie of breed kenniswerk.
- Tegenargument in de aflevering: zelfs als één model het niet kan, kan een ensemble van modellen + softwarelagen (agents, tools, geheugen) wél richting dat niveau groeien.
- Poetic wordt gepositioneerd als bewijs dat “compound AI” (teams van AI’s, scaffolding) grote sprongen kan veroorzaken zonder nieuw foundation model.

# Standaarden en interoperabiliteit: MCP naar de Linux Foundation
- Nieuws: Anthropic, OpenAI en Block bundelen krachten rond open AI-standaarden.
- Anthropic doneert Model Context Protocol (MCP) aan een foundation onder de Linux Foundation (nonprofit governance).
- Relevantie:
  - MCP wordt neergezet als een soort “HTTP voor AI-integraties”: een universele manier voor AI-applicaties/agents om met externe systemen te praten.
  - Genoemde adoptie: >10.000 actieve MCP-services en “ontzettend veel” MCP-calls; breed gedragen door grote modelbouwers.
  - Steun van grote partijen: Google, Microsoft, AWS, Cloudflare.
- Waarom belangrijk:
  - Versnelt plugin/directories en maakt koppelingen eenvoudiger voor eindgebruikers (Notion, Google Drive, Canva, Figma, domotica zoals “verwarming harder zetten”).
  - Verlaagt lock-in: standaarden onder neutrale governance maken brede adoptie aantrekkelijker.
- Extra context: Google’s A2A (agent-to-agent) protocol wordt genoemd als parallel initiatief om agents met elkaar te laten communiceren.

# Agency-case: AI Guardrails voor merkveilige klantinteractie
- Dept introduceert “AI guardrails” als oplossing om consumentinput te controleren zodat chatbots/AI-ervaringen merkveilig blijven.
- Probleem:
  - Consumenten kunnen gevoelige data, politieke statements, verboden content of concurrentnamen invoeren.
  - AI kan hallucineren of “meegaan” met ongewenste meningen.
- Oplossing/workflow:
  - Een extra controlelaag over het inputveld die realtime classificeert of input binnen toegestane grenzen valt.
  - Pas na “veilig” signaal mag de generatieve AI het antwoord formuleren.
- Implementatie-aspecten:
  - Eerst beleid definiëren (90% logisch, 10% merkspecifieke randgevallen zoals concurrenten).
  - Model trainen/afstellen, iteratief testen.
  - Doel: veilig, consistenter, merkconform en schaalbaar voor customer interaction/service/campagnes.

# Getipte tool: Tasklin (agentplatform met MCP-koppelingen)
- Tool: Tasklin, platform om AI-agents te maken in gewone taal (Nederlands), zonder programmeren en zonder “blokjes slepen”.
- Kernfunctie: eenvoudig koppelen van tools via MCP (integraties als Gmail etc.).
- Geteste use-case (door redacteur Shank):
  - Dagelijkse AI news briefing automatisch in je inbox.
  - Setup in ~2 minuten: schema, e-mailadres, bronnen.
  - Output: gestructureerde mail met categorieën zoals doorbraken, investeringen, beleid.
  - Iteratieve verbetering via chat: na feedback (“ik wil links”) werden volgende mails automatisch mét werkende links verstuurd.
- Extra genoemde use-cases:
  - Automatisch achtergrondinformatie toevoegen bij agenda-afspraken over gesprekspartners.
  - Wekelijkse statusupdates automatisch laten versturen.
- Prijsmodel:
  - Niet goedkoop; gratis gebruik beperkt.
  - Betaalde abonnementen vanaf $35/maand.
- Positionering: rendabel bij voorspelbaar, herhaalbaar handwerk (informatie sprokkelen, researchroutines, reporting).

# AI en energie-economie: datacenters slokken infrastructuur op
- Nieuws/observatie: AI-datacenters trekken zoveel stroomcapaciteit naar zich toe dat ze concurreren met andere industrie.
- Bitcoin miners worden opgekocht door AI-partijen vanwege hun waarde: betrouwbare stroomaansluitingen.
- Voorbeeld: Boom Supersonic (supersonisch vliegtuigproject) gaat gasturbines (42 MW) verkopen aan datacenters om cashflow te genereren; jet engines in containers die kerosine verbranden voor elektriciteit.
- Economisch concept: “crowding out” (één sector absorbeert kapitaal, stroom, arbeid, industriële capaciteit).
- Maatschappelijke spanning: de verhouding tussen “jet engines voor synthetische video/slop” versus “maatschappelijke/medische doorbraken” moet kloppen om legitimiteit te houden.

# Experiment van Anthropic: research-chatbot die een echt gesprek emuleert
- Tool/experiment: een tijdelijke research-interface van Anthropic (stond ~1 week online, daarna offline).
- Doel: kwalitatief onderzoek naar hoe mensen AI gebruiken en hoe ze zich erbij voelen (impact op werk/leven), naast kwantitatieve usage-metrics.
- Probleem met standaard surveys/chatbots: saai, lage motivatie, mensen antwoorden niet uitgebreid.
- Nieuwe workflow:
  - Chatbot voert een inhoudelijk gesprek op jouw niveau (zoals iemand uit je vakgebied op een conferentie).
  - De bot houdt het gesprek gaande, prikt door, stelt vervolgvragen als een interviewtechniek.
  - Rolomkering: de bot “activeert” jou met vragen; niet alleen jij die vragen stelt.
  - Opvallend: de bot geeft ook feedback/tegenargumenten terug, waardoor het gesprek wederkerig voelt en meer engagement oplevert.
- Implicatie:
  - “Telefonische enquête on steroids”: organisaties kunnen eerlijkere, diepere antwoorden krijgen.
  - Past in het bredere punt: met prompt/flow en UX kun je met hetzelfde onderliggende model een totaal andere ervaring creëren.

# Praktische AI-workflow in woningmarkt: Walter Living + agent met databronnen
- Casus: Walter Living (woningrapporten) duwt een chatbot-ervaring naar voren.
- Eerst weerstand (“geef mij gewoon PDF’s”), maar daarna blijkt het krachtig door “grounded agent”-gedrag:
  - De bot haalt op de achtergrond data op uit relevante bronnen (zoals Funda, Kadaster-achtige data/verkopen).
  - De interface laat zien wat hij doet (transparantie/trace van acties).
  - Interactief advies: signaleren van “lokkertjesprijs”, zoeken naar alternatieve woningen met realistischer prijsstelling, etc.
- Belang: voorbeeld van de verschuiving van “AI-bolletje in de hoek” naar een echt op maat gemaakte workflow die probleemgericht is, mét betrouwbare externe data-integraties.

# Uitgevers/journalistiek als volgende integratiegolf (wensbeeld)
- Behoefte: een AI die wél mag putten uit betaalde archieven/kwalitatieve bronnen (Volkskrant/Trouw/Parool, Consumentenbond), i.p.v. alleen open web.
- Gewenste workflow:
  - Gebruiker betaalt voor bronnen (abonnementen).
  - AI doet via standaarden (zoals MCP) gecontroleerde calls naar die bronnen en syntheseert antwoorden met brondiversiteit (ook conflicterende inzichten).
  - Desnoods via microtransacties per artikel/broncall.
- Onderliggende boodschap: de waarde zit in betrouwbare data + goede integratie, niet alleen in het taalmodel.

# Programma’s, tools en workflows (overzicht)
- ChatGPT (OpenAI): geruchten GPT-5.2; advertentietest uitgezet; pop-up “hoe wil je dat we tegen je praten?” als voorbeeld van product-iteratie/UX tuning.
- Gemini 3 Pro (Google): gebruikt als foundation model door Poetic; baseline waar scaffolding omheen wordt gebouwd.
- Slack: ontvangt Cloud Code-integratie; AI taggen in chats voor debug/vibe coding.
- Cursor / GitHub Copilot: genoemd als tools met (of rond) Slack-integraties; competitie op workflow-integratie.
- MCP (Model Context Protocol): standaard voor AI ↔ externe systemen; basis voor plugin-ecosystemen en agentkoppelingen.
- A2A (Agents-to-Agents, Google): protocol voor agent-onderlinge communicatie, als complement/parallel aan MCP.
- Tasklin: no-code/low-code agentplatform; bouwt agents in natuurlijke taal; koppelt via MCP aan tools (bv. Gmail) voor geautomatiseerde briefings en workflowtaken.
- Walter Living: woningadviesplatform; verschuift van PDF-rapporten naar interactieve agent-UX met gekoppelde databronnen.
- Anthropic research-chatbot (tijdelijk): kwalitatieve interview-bot die engagement verhoogt door gesprekstechniek en wederkerigheid.
- Dept “AI Guardrails”: workflowlaag voor realtime inputfiltering en merkveilig genereren in chatbots/klantinteractie.

# AI-gerelateerd nieuws (samengevat)
- Poetic >50% op Arc AGI 2 met Gemini 3 Pro + scaffolding (grote benchmark-sprong buiten Big Tech).
- GPT-5.2 als snelle tussenrelease; advertenties in ChatGPT tijdelijk stopgezet na klachten.
- Cloud Code-integratie naar Slack: vibe coding direct in werkchat.
- MCP gedoneerd aan Linux Foundation; brede adoptie en steun door grote techpartijen.
- Energie-infrastructuur verschuift richting AI: overnames van bitcoin miners voor stroomaansluitingen; Boom verkoopt 42MW-gasturbines aan datacenters.