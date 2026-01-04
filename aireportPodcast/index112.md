# 112. BONUS: het laatste webinar met onze AI-wensen voor 2026 + unified agent interfaces + Wietses verj... (2025-12-17) [link](undefined)


 Praktische inzet van AI in organisaties en onderwijs: hoe je betrouwbaarheid verhoogt (minder hallucinaties), tools/flows kiest en bouwt (no/low-code, agents, workflows), en welke richting de AI-markt opgaat (open modellen, lokale AI, copilots en workflow-bouwers).

# Belangrijkste thema’s en onderwerpen
- Aankondiging van nieuwe masterclasses (AI-skill in 1 uur) met focus op “programmeren met AI”.
- Hallucinaties beperken in LLM’s: grounding, RAG, tool calling, multipass/flow-architecturen, multimodel-strategieën en trade-offs (snelheid/kosten vs betrouwbaarheid).
- Wensen/verwachtingen voor 2026: proactieve agents met een goede “unified interface” en lokale AI die slim genoeg is om het internet te gebruiken wanneer nodig.
- Workflow tools in de ecosystemen van Microsoft en Google (Copilot Workflows, Google’s workflow-achtige builder voor Workspace) en de beperkingen van integraties/connectors.
- Onderwijs: docenten die zonder programmeerkennis agents/workflows willen bouwen, binnen AVG en in een afgeschermde schoolomgeving; afhankelijkheid van LMS-leveranciers en gebrek aan open integraties.
- Tool-keuze en “tool fatigue”: omgaan met snelle veranderingen, vermijden van lock-in, werken met standaarden/protocollen en toekomstbestendige werkwijzen.
- Nieuws/ontwikkelingen: Mistral’s (grote) open model, enterprise positionering, discussie over leeftijdsrestricties social media (Australië), Google als “vibe winner” qua shipsnelheid.

# Masterclass en aanbod (gebruiksscenario + tool)
- **Masterclass (8 januari, 12:00; exclusief voor betaalde abonnees)**: “Cloud Code” als tool om als beginner “from scratch” met AI te leren programmeren.
- **Doel**: een idee voor een tool/app omzetten naar een werkend prototype (web/app) met aandachtspunten voor opzet en realisatie.
- **Doelgroep**: expliciet beginners zonder technische achtergrond.
- **Commercieel aanbod**: oudejaarsactie voor jaarabonnement (tijdelijk tarief) met toegang tot de masterclass.

# Hallucinaties: technieken, workflows en praktische toepassing
- **Grounding via tool calling (web/zoekfunctie) als harde eis in systeemprompt**
  - Aanpak: in de systeemprompt opnemen dat *elke feitelijke claim* gecontroleerd moet worden door een tool (web/zoek/grounding).
  - Effect: minder hallucinaties omdat het model niet “zelf” hoeft te beslissen wanneer het onzeker is; het *moet* altijd checken.
  - Trade-off: antwoorden worden trager (soms minuten). Belangrijk om eindgebruikers te informeren dat er “onderzoek” wordt gedaan.
  - Tools/varianten die genoemd worden: web-grounding via o.a. Anthropic/Sonnet-achtige webcontext of “gewoon Google gebruiken”.

- **RAG (Retrieval-Augmented Generation) in zakelijke context**
  - Gebruiksscenario: support/klantenservice-automatisering op basis van een interne FAQ of documentset.
  - Praktische vorm: “vinkjes” in een copilot-omgeving waarbij je een map (bijv. OneDrive) koppelt; achter de schermen wordt context opgehaald (RAG).
  - Beperkingen: standaard enterprise-oplossingen zijn vaak geoptimaliseerd voor snelheid → minder kritisch → meer kans op bluffen.

- **Multipass/flow-architectuur (“slang van blokjes”)**
  - Kernidee: splits taken in meerdere stappen met verschillende rollen voor modellen.
  - Voorbeeldworkflow (podcast/transcript-samenvatting):
    1. Transcriberen
    2. Samenvatten
    3. Claims distilleren uit samenvatting
    4. Per claim checken: komt dit uit transcript of is het “bijbedacht”?
    5. Herschrijven met alleen geverifieerde claims/facts
  - Observatie: een aanzienlijk deel van claims kan “bijgevuld” zijn door het model; multipass maakt dit zichtbaar en corrigeerbaar.
  - Optimalisatie: per blok een ander model kiezen (kleine/goedkope modellen voor “fact extraction”, zwaardere reasoning voor synthese).
  - Trade-off: betrouwbaarder, maar trager (meerdere minuten) → geschikt voor achtergrondprocessen, minder voor realtime apps.

- **Multimodel aanpak (“council of LLMs”)**
  - Vraagstuk: meerdere modellen (bijv. Gemini + ChatGPT) bevragen om fouten te reduceren.
  - Nuance: modellen delen vaak trainingsdata/valkuilen; ze kunnen elkaars fouten bevestigen. Niet gepresenteerd als “silver bullet”.

- **Modelkeuze en hallucinatiebenchmarks**
  - Genoemd: **GPT-5.1** scoort volgens “system card”/benchmarks beter op hallucinaties, vooral in “thinking high”/reasoning modus.
  - Trade-offs: hogere kosten en langere wachttijd (± 30s of meer).

# Wensen voor 2026: agents, UI en proactieve assistentie
- **Behoefte aan goede UI voor agents**
  - Situatie: modellen (zoals Opus 4.5 genoemd) zijn sterk in programmeren en iteratief problemen oplossen, maar de gebruikerservaring voor “agents die op de achtergrond werken” is nog zwak.
  - Gewenste workflow: AI observeert werkcontext (meetings, e-mails, afspraken, routinehandelingen), vist follow-ups eruit, en presenteert ’s ochtends een actielijst:
    - ✅ uitvoeren
    - ❌ negeren
    - ✏️ bewerken
  - Kernpunt: “unified interface” voor meerdere agents en taken, proactief in plaats van reactief.

# Lokale AI en hybride (on-device + internet) workflows
- **Demo-scenario op verjaardagen: Local AI op iPhone in vliegtuigmodus**
  - Tool: **“Locally AI”** (iPhone app) waarmee een model lokaal draait zonder internet.
  - Waardepropositie: privacy (data blijft lokaal), energie/lokale verwerking, en (idealiter) training op “open data” (commons/“data uit het park”).
  - Beperkingen nu: lokale modellen zijn “niet zo heel slim” en kunnen (nog) niet toolcallen/internet op.

- **Android alternatief**
  - Tool: **Google Edge AI** (GitHub) als app/omgeving om lokale modellen te draaien en ermee te experimenteren.

- **Grote wens: tool calling op device**
  - Doel: een klein lokaal model dat “weet wat het niet weet” en dan:
    - zelf het internet op gaat (Wikipedia/Google)
    - of een “grotere broer/zus” in de cloud raadpleegt (hybride model; referentie aan Apple’s hybride benadering)
  - Praktisch resultaat: “grounding met één knop” op je telefoon; meer taken lokaal, maar toch up-to-date via just-in-time retrieval.

# Copilot Workflow Tools en no/low-code flowbuilding
- **Microsoft Copilot Workflows (genoemd als nieuw)**
  - Positionering: visuele flowbuilder vergelijkbaar met **n8n** (blokken/agentic flows).
  - Gebruiksscenario (voorbeeld): in Outlook komt een kritieke mail binnen → flag → notificatie naar Teams.
  - Belangrijk onderdeel: **predefined connectors** naar Microsoft-ecosysteem (OneDrive/Office/Outlook/Teams); vergelijkbaar met wat zij “connectors” noemen en in de AI-wereld ook als tool/MCP-achtig wordt gezien.

- **Google’s workflow-builder voor Workspace (nieuw genoemd, gezien “deze week”)**
  - Concept: flows bouwen met natuurlijke taal (“als dit gebeurt, doe dat; gebruik Gemini hier”).
  - Beperking: weinig externe integraties; deals met o.a. Asana en Salesforce, maar niet met allerlei andere tools (zoals Notion genoemd).
  - Kritiek: grote platformen focussen op eigen tooling, minder op brede open integratie.

# Desktop-automatisering en MCP-integraties (lokale workflows)
- **Beeper (multimessenger) + MCP**
  - Gebruiksscenario: AI-model kan met Beeper interacteren via MCP (berichten lezen/schrijven), maar dit werkt vooral als de app lokaal open staat.
  - Probleem: cloudgebaseerde agents zijn handig (laptop hoeft niet aan), maar kunnen niet bij lokale apps die je niet in de cloud wilt.

- **Wens: “n8n/Lindy, maar dan op mijn machine”**
  - Doel: lokale flow-automatisering die met desktop-apps kan interacteren (vergelijking met Apple’s Shortcuts/Automator).
  - Gewenste richting: AI die via “computer use”/accessibility-achtige besturing door interfaces kan klikken als er geen officiële connectors zijn.

# Onderwijs: docenten-agents zonder programmeerkennis, AVG en schoolomgeving
- **Vraag**: docenten willen zelf agents bouwen voor lesvoorbereiding, feedback, toetsing, oefenmateriaal; AVG-proof en liefst on-premise/afgeschermd.
- **Realiteit volgens gesprek**:
  - Veel hangt af van de bestaande “stack”: Google/Microsoft omgeving + LMS (Canvas/Blackboard/etc.).
  - Essentiële vraag: zijn er connectors naar het LMS? Zo niet, dan blijft het copy-paste of maatwerk.
  - “Make vs buy”: zelf knutselen (bijv. n8n in Docker containers) of leveranciers dwingen/vragen om integraties (MCP/connector-roadmaps).
  - Kritiek op LMS-/onderwijssoftwaremarkt: traag, weinig concurrentie, gesloten systemen; privacy-vereisten kunnen ook als rem/vertragingsmechanisme werken.
- **Alternatieve (radicale) workaround**:
  - “Computer use” lokaal: AI rond laten klikken in Canvas/LMS om data te exporteren/importeren zonder officiële API/connector; lokaal opslaan voor gesprek/RAG.
- **Didactische inzet van AI bij feedback (concreet gebruiksscenario)**
  - AI als “buddy/collega” die docenten helpt betere feedback te formuleren.
  - Belangrijk: niet alleen feedback doorsturen, maar docent laat AI stap-voor-stap uitleggen *waarom* die feedback passend is (docent leert mee).
  - Motivatie: essays nakijken is intensief; AI kan helpen focus op inhoud te houden en consistentie te verhogen.

# Mistral open source: betekenis en marktimplicaties (AI-nieuws)
- **Nieuws**: Mistral brengt **Mistral Large 3** direct open source uit (Hugging Face-download impliciet genoemd).
- **Interpretatie**:
  - Mistral vergelijkt vooral met andere open modellen; minder met top gesloten frontier-modellen (GPT-5.1/Opus 4.5) omdat het daar minder competitief zou zijn.
  - Open model is niet “gratis zonder voorwaarden”: licenties kunnen betaling vereisen bij grootschalig commercieel gebruik (bijv. datacenters).
  - Strategische pivot: minder meedoen aan “frontier closed model race”, meer richting enterprise, open modellen als “grondstof” voor fine-tuning, en partnerships (genoemd: samenwerking met **SAP**).
  - Breder patroon: open modellen (o.a. Chinese) worden gebruikt als basis door bedrijven die er een fine-tuned product van maken en doorverkopen; Mistral positioneert zich ook als zulke basislaag.

# Leeftijdsrestricties, AI en media (AI-gerelateerd nieuws/maatschappij)
- **Australië**: invoering leeftijdsrestrictie social media (tot 16); platforms verantwoordelijk voor controle/naleving.
- **EU/Europa**: verwachting dat vergelijkbare regelgeving volgt; discussie draait om *handhaving* en leeftijdsverificatie.
- **Mogelijke (controversiële) handhavingsmethode**: AI die leeftijd inschat op basis van gedrag (privacy/ethische haken en ogen).
- **AI en kinderen**:
  - Geen eenduidig advies; nadruk op samen gebruiken (“handje vasthouden”) en focus op “lean forward” gebruik: creëren/bouwen (muziek, beelden), niet passief consumeren.
  - Belang van AI-/digitale geletterdheid: kinderen voorbereiden op algoritmen en gepersonaliseerde feeds; anders is de sprong op 16 jaar te groot.

# Google en onderwijs (tools en experimenten)
- **Chromebooks in scholen**: aannemelijk dat Gemini-integratie toeneemt; discussie over wenselijkheid als één bedrijf te dominant wordt.
- **NotebookLM** (grounded op eigen bronnen) als basis:
  - Gebruiksscenario: eigen bronnen uploaden → samenvatten/vragen beantwoorden/podcast genereren.
  - Nieuwe functie genoemd: **knowledge cards/flashcards** genereren voor leren en toetsen.
- **Experiment**: “NotebookLM for Education” (regiorestrictie genoemd) waarin lesmateriaal mogelijk automatisch gegenereerd wordt (slides, voice-overs, cards).
- **Visie**: Google kan industrie “wakker schudden”, maar het is onwenselijk als Google de dominante lesmethode-maker wordt; bovendien is onderwijs voor Google mogelijk economisch relatief klein.

# Prompt- en projectorganisatie: één grote prompt vs gestructureerde instructies
- **Advies**: liever “slicen” (meerdere kleine instructies/skills) dan één mega-prompt.
- **Reden**: voorkomen van “prompt infighting” (instructies die elkaar tegenspreken of onduidelijk overlappen) en betere debugbaarheid.
- **Voordeel van multipass**: je ziet waar kwaliteit/data verloren gaat en kunt per stap optimaliseren.

# Claude “skills” en programmeertools (workflow)
- **Skill-concept**: een “skill” is in praktijk een bundel van prompts + eventueel code/tooling; providers leveren standaardskills (bijv. frontend bouwen).
- **Gebruik**:
  - Sprekers bouwen liever in echte dev-omgevingen en AI-code tools (cursor/windsurf/terminal-achtige workflows) dan in de ingebouwde frontend-skill.
  - Reden: snel uit het “jasje” van standaardskills groeien; behoefte aan controle en herbruikbare structuren.

# Onderzoeksvraag: Chain-of-Thought vs few-shot bij tekstclassificatie
- Vraag gaat over accuraat classificeren (sentiment/cynisme/etc.) en mogelijke ruis door Chain-of-Thought.
- Antwoord in de sessie: geen definitief standpunt; suggestie dat gespecialiseerde (kleinere) classificatiemodellen of fine-tuned modellen bestaan (Hugging Face-categorie), maar geen uitgewerkt recept.

# Toolkeuze zonder verlamd te raken: praktische strategie
- **Context**: veel toolsets (n8n, Claude, CLI, Cursor, etc.) veranderen snel; risico op “verlamming” door keuze-overload.
- **Aanpak**:
  - Speel aan de “bleeding edge” om te begrijpen wat kan, maar accepteer dat tools tijdelijk zijn (lage loyaliteit).
  - Tegelijk inzetten op toekomstbestendigheid: documentatie, tests, en architectuur die modelwissels mogelijk maakt (anti lock-in).
  - Standaardisatie in opkomst:
    - project-specifieke instructiebestanden (bijv. **claude.md** genoemd)
    - beweging richting generiekere instructiestandaarden (bijv. **lm.md** genoemd)
- **Pragmatische motivatie voor toolkeuze**: soms kies je een tool omdat die toegang geeft tot een bepaald topmodel (bijv. Gemini “thinking high”) en testkwaliteit (zoals tests schrijven) verbetert.

# Overkoepelend sentiment en observaties
- Publiek/organisaties lijken “wakkerder” dan een jaar geleden; vragen worden inhoudelijker.
- Negatief maatschappelijk sentiment rond AI komt mede door “AI slop”, deepfakes en informatie-erosie; behoefte aan betere taal om subdomeinen van “AI” uit elkaar te trekken (zoals onderscheid internet vs social media).
- Tegelijk zijn er doorbraken met potentieel grote maatschappelijke waarde (medische toepassingen, wetenschappelijke versnelling), maar die raken ondergesneeuwd in de containerterm “AI”.

# Afsluitende planning
- Aankondiging van een volgend webinar (donderdag 8 januari 2026, 12:00) en herhaling van de abonnementsactie als toegangspoort tot deelname.