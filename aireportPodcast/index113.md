# 113. Hoe één baan in 18 maanden totaal veranderde (2025-12-18) [link](undefined)


 De snelle verschuiving in kenniswerk door AI—met softwareontwikkeling als voorhoede—waarbij “programmeren” steeds meer verandert in het aansturen, controleren en orkestreren van AI-agents en workflows, en eindgebruikers steeds makkelijker zelf software en automatiseringen kunnen creëren.

# Belangrijkste thema’s en onderwerpen
- Versnelling van AI-capaciteiten (grotere context, betere coherentie, sneller beeldbewerken) en de impact daarvan op werkprocessen  
- “Vibeshift” bij softwareontwikkelaars: van zelf code schrijven naar prompts geven, wachten en sanity-checken  
- Democratisering van software: eindgebruikers worden makers door AI-tools met integraties en agent-workflows  
- Scaffolding/harnas rond modellen (tools die testen, debuggen, bestanden openen, documentatie raadplegen, subagents inzetten) als cruciale versneller naast modelverbeteringen  
- Nieuwe spanning tussen procesgerichte vakmensen (die het maakproces waarderen) en eindresultaatgerichte gebruikers (die vooral output willen)  
- Onderwijs (met name HBO) als kwetsbare schakel: betere deliverables, maar afnemende “intuïtie/vaardigheid” bij studenten en toetsing die niet meer past  
- Brede maatschappelijke vraag: wat gebeurt er als mentale arbeid (denken/produceren van informatie) net zo automatiseerbaar wordt als fysieke arbeid?

# AI-gerelateerd nieuws
- Google Translate: live vertaling via oordopjes (VS en India), met behoud van intonatie/tempo/toonhoogte; uitrol op iOS/Android/web, nog niet in Nederland (wel verwacht volgend jaar).  
- OpenAI GPT 5.2: verbeterd omgaan met grote hoeveelheden tekst/data; kan o.a. hele jaarverslagen/spreadsheets in één keer analyseren zonder de “draad kwijt te raken”.  
- ChatGPT Images 1.5: tot 4× sneller, kan bestaande foto’s bewerken via natuurlijke taal (stijl wijzigen, objecten toevoegen) met minder “detailverlies”; vergelijking met Google’s “Nano Banana Pro” (beter bij complexe infographics/presentaties volgens Ethan Mollick).  
- Disney x OpenAI: driejarige deal voor genereren van video’s met 200+ Disney/Marvel/Pixar/Star Wars-personages via Sora; gezichten/stemmen van echte acteurs uitgesloten; Disney investeert $1 miljard en rolt ChatGPT intern uit.  
- Time Magazine: “architecten van AI” als Person of the Year 2025 (o.a. leiders van Nvidia, OpenAI, Google DeepMind, Anthropic, Elon Musk).

# Gebruikte programma’s en concrete gebruiksscenario’s
- Tasklet (tool met ingebouwde integraties)
  - Scenario: vergaderingen automatisch laten transcriberen (via Notion), daarna:
    - Actiepunten extraheren en sorteren per verantwoordelijke
    - Herkennen van “dingen die het zelf kan doen” en die direct uitvoeren
    - Automatisch e-mailconcepten maken op basis van besproken punten (bijv. “we moeten Annet mailen met X/Y/Z”), klaarzetten als draft; gebruiker controleert en vult adres/finetuning in
    - Automatisch vervolgmeeting plannen wanneer in de meeting blijkt dat iets later vervolgd moet worden; inclusief “briefing” in een mail aan jezelf met samenvatting en voorstelagenda
  - Belangrijk detail: de gebruiker bouwt niet expliciet integraties of flows; de tool abstraheert het “programmeren” weg door subagents te genereren vanuit natuurlijke taal en context.

- Notion (transcriptiebron)
  - Scenario: Notion transcribeert meetings; Tasklet haalt transcript eruit en verwerkt dit naar acties, mails en vervolgafspraken.

- OpenAI “platform met blokjes” (visuele agentbouw)
  - Scenario: agents bouwen via drag-and-drop/flows; in gesprek wordt dit gezien als “nog te veel werk” vergeleken met tools die de extra abstractiestap al nemen (zoals Tasklet).

- Cloud Code + Claude Opus 4.5 (Anthropic) als programmeerstack
  - Scenario voor ontwikkelaars: niet meer handmatig coderen, maar:
    - Prompten in een code-omgeving
    - AI laat code draaien, leest errors, past aan, test opnieuw (trial-and-error loop)
    - Ontwikkelaar sanity-checkt en grijpt in bij randgevallen/veiligheid/architectuur
  - Scenario voor niet-programmeurs/beginners: leren om met AI websites/tools/apps te bouwen zonder klassieke programmeerachtergrond.

- Codex (OpenAI) als programmeer-tooling
  - Scenario: vergelijkbaar met Cloud Code in het automatiseren van “aanpassen-testen-herhalen” en het overnemen van copy-paste debugging workflows.

- Cursor (genoemd als tool in de tweet)
  - Scenario: prompting + code laten genereren/aanpassen, vervolgens controleren; onderdeel van dezelfde “prompt → output → sanity check” werkstijl.

- BitRig (iOS-app; “App Store in prompten”)
  - Scenario: gebruiker beschrijft in chat wat voor app nodig is (bijv. “een klok met paarden om mijn dochter klok te leren kijken”) en krijgt binnen ~30 seconden een echte iOS-app (Swift/SwiftUI), te distribueren via TestFlight en potentieel te publiceren in de App Store.

- Gemini (Google) in onderwijs/quiz-scenario
  - Scenario: lesmateriaal invoeren en prompt “maak een toets”; output bevat een complete quiz-ervaring (multiple choice, feedback, score bijhouden, herhaling fout beantwoorde vragen). Dit illustreert “one-shot” output die ver gaat zonder uitgebreide prompting.

- Google “Agent to UI (A2UI)” (concept/demo genoemd)
  - Scenario: interfaces “just in time” genereren op basis van gesprek; knoppen/UI ontstaan on-the-fly terwijl je praat met je telefoon—richting gepersonaliseerde, dynamische apps.

- Bol “AI cadeauhulp” (conversational shopping)
  - Scenario in Bol-app: gebruiker beantwoordt vragen over ontvanger (hobby’s, relatie, voorkeuren/afkeuren, budget). AI stelt vervolgvraagjes en geeft cadeau-suggesties die direct te bestellen of op een wensenlijst te zetten zijn.
  - Positionering: eerste stap naar een bredere “conversational shopping journey” op basis van productkennis, reviews en assortimentdata.

# Nieuwe tools en AI-workflows (uitgebreid)
- Meeting → transcript → acties → uitvoering (agentic meeting opvolging)
  - Workflow: audio/meeting → transcriptie (Notion) → agent leest transcript → haalt actiepunten & verantwoordelijkheden → detecteert uitvoerbare taken (e-mail drafts, afspraken plannen) → voert taken uit of zet ze klaar → vraagt om bevestiging (“zal ik dit doen?”) of meldt “ik heb dit gedaan”.
  - Vernieuwing: niet alleen samenvatten, maar post-meeting uitvoering door agents.

- Scaffolding/harnas rond code-modellen (evolutie in ~18 maanden)
  - Van: copy-paste code in ChatGPT → suggesties terugplakken → runnen → errors terugplakken  
  - Naar: geïntegreerde tools (Copilot/Cursor/Codex/Cloud Code) die:
    - Zelf code plaatsen in juiste files
    - Error logs meelezen
    - Autonoom itereren (patch → test → patch)
    - Relevante bestanden/documentatie openen
    - Meerdere subagents parallel inzetten (documentatie, security, accessibility)
    - Eerst een plan schrijven en dat plan laten uitvoeren
  - Resultaat: “manageren” van agents i.p.v. zelf typen; meer focus op orkestratie en kwaliteitscontrole.

- Persoonlijke “scaffold” via GPT 5.2 prompting guide + custom instructions
  - Workflow: GPT 5.2 vraagt om “custom instructions” te genereren op basis van:
    - wat ChatGPT al over je weet
    - de officiële GPT-5 prompting guide
  - Doel: toekomstige gesprekken standaard beter laten aansluiten op je werk en taken (een permanente personalisatie-laag).

# Impact op softwareontwikkeling (“vibeshift”)
- Werk verandert inhoudelijk: van geconcentreerd coderen naar een loop van aanzetten → wachten → controleren → bijsturen.  
- Twee groepen:
  - Vibecoders/eindgebruikers: konden niet programmeren, kunnen nu wel (via abstractie en agents).
  - Professionele developers: zien steeds meer “onmogelijkheden” verdwijnen; verschuiven naar regie, review, architectuur, randgevallen, veiligheid.
- Niet alle software is even geraakt:
  - Gespecialiseerde/veiligheidskritische embedded/industriële systemen blijven lastig (weinig trainingsdata, hoge betrouwbaarheidseisen).
  - “Midden van de curve” (dashboards, CRUD, databases, standaard web/app werk) is het meest automatiseerbaar en ziet nu de grootste versnelling.
- Nieuwe bottleneck: menselijke context/intuïtie
  - AI kan een codebase snel “begrijpen”, maar de menselijke dirigent kan het tempo en volume niet bijhouden.
  - Als agents heel veel bouwen, mist zelfs een senior soms de intuïtieve kennis die je normaal opbouwt door jaren in de code te zitten.
  - Daarom worden documentatie en uitleg-artefacten steeds belangrijker als onderdeel van de scaffold.

# Onderwijs en arbeidsmarkt (signalen en zorgen)
- HBO-docenten ervaren dat portfolio’s massaal AI-gegenereerd zijn:
  - Deliverables ogen beter, maar studenten kunnen vaak niet uitleggen wat ze “gemaakt” hebben (verlies van begrip/intuïtie).
  - Instellingen hebben beperkte prikkels om massaal te laten zakken; hierdoor dreigt de lat voor studentcompetentie te dalen terwijl outputkwaliteit stijgt.
- Breder dilemma:
  - Zelfs als onderwijs zich aanpast en studenten beter worden met AI, kan de arbeidsmarkt minder behoefte hebben aan mensen voor werk dat “door glasvezel kan” (informatiewerk dat volledig digitaal overdraagbaar is).

# Centrale vragen die op tafel blijven
- Wat blijft structureel menswerk (randgevallen, veiligheid, context uit de fysieke wereld, fuzzy besluitvorming, sociale/juridische processen)?  
- Wanneer verschuift het van “kan het?” naar “is het breed uitgerold?” (diffusie vs. capability)?  
- Wat betekent het maatschappelijk als steeds meer mensen “naast de machine” komen te staan in plaats van “in de machine” mee te draaien?