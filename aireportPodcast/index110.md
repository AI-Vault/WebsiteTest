# 110. Alexander kan eindelijk programmeren + DeepSeek haalt Amerikaanse modellen in + de 'ziel' van Cla... (2025-12-04) [link](undefined)


 Snelle verschuivingen in het AI-landschap: open-source modellen (DeepSeek, Mistral) winnen terrein en worden “onder de motorkap” breed ingezet; tegelijk professionaliseert Anthropic zijn ontwikkel- en platformstrategie (Claude/Claude Code, overname Bun) en lekt er een intern “ziel”-document dat laat zien hoe Claude tijdens training gevormd is. Daarnaast speelt AI-veiligheid een rol via een klokkenluiderszaak rond humanoid-robots.

# Belangrijkste thema’s en onderwerpen

# 1) “Democratisering” van software bouwen met Claude Opus 4.5, Claude Code en Cursor
- Ervaring: een niet-programmeur ontdekt dat AI-coded tooling nu zó gebruiksvriendelijk is dat hij daadwerkelijk werkende software kan bouwen.
- Kernobservatie: Claude Opus 4.5 voelt niet alleen beter in benchmarks, maar vooral praktisch betrouwbaarder bij software bouwen; eerdere pogingen liepen vaak vast, nu “klikt” het.
- Belangrijke nuance: tooling is minder intimiderend geworden doordat interfaces code verbergen en de gebruiker vooral in chat + live preview werkt.

# 2) Concrete gebruiksscenario’s: van e-mail triage tot podcast-automatisering
- Voorbeeld (CPO Webflow): gebruikt Cursor met “agents” in een terminal/CLI-achtige interface om werkprocessen te automatiseren:
  - E-mail triage: mail doornemen, prioriteren, archiveren, beantwoorden.
  - Meeting-voorbereiding: samenvatten wat er vorige keer is besproken, context klaarzetten voor komende meeting.
  - LinkedIn-post schrijven: concepten genereren en afwerken.
  - Agenda-optimalisatie: agent die op basis van doelstellingen adviseert welke dagen “meetingvrij” moeten blijven.
- Eigen project (podcast workflow): een tool gebouwd die:
  - Podcasts downloadt,
  - Transcribeert,
  - Tekst “hertaalt”/transformeert van transcript naar leesbaar journalistiek artikel.
  - Extra gewenste uitbreiding: caching/archivering (niet opnieuw downloaden), wat impliceert: storage + database + cloud hosting.
- Delen en uitrollen: discussie over stap van lokaal op laptop naar publiceren (GitHub commit, deploy naar web/URL).

# 3) Anthropic neemt Bun over: signaal richting “AI + hostingplatform” en nieuwe inkomstenstromen
- Bun: cruciaal infrastructuur-onderdeel in moderne JavaScript/ontwikkeltooling (belangrijk binnen developer-ecosystemen; genoemd als essentieel ingrediënt voor Claude Code).
- Waarom strategisch:
  - Niet alleen developer tooling, maar richting “just-in-time maatwerksoftware” voor niet-programmeurs.
  - Mogelijke volgende stap: van “artifacts” (losse output) naar volledig te publiceren tools op een URL, draaiend in Anthropic’s cloud.
  - Verdienmodelhypothese: naast tokens/abonnementen ook revenue share op start-ups/individuen die tools bouwen en hosten via Anthropic.
- Use case visie: gebruiker zegt in natuurlijke taal “zorg dat deze podcast niet opnieuw gedownload wordt”; platform regelt automatisch storage/object storage/database zonder dat de gebruiker AWS/S3 hoeft te kennen.

# 4) Open-source modellen in opmars: DeepSeek terug met V3.2 en de geopolitieke realiteit “onder de motorkap”
- DeepSeek V3.2:
  - Open source (gratis te downloaden, lokaal/privé te draaien, aan te passen).
  - Prestaties volgens tests: in de buurt van “frontier” gesloten modellen (OpenAI/Gemini).
  - Reasoning traces: DeepSeek laat innerlijke redenering opvallend open zien, wat gebruikers fascinerend vinden.
- MIT-onderzoek (AI-gerelateerd nieuws):
  - Chinese open-source modellen zouden VS hebben ingehaald in wereldwijde downloads: 17% China vs 16% VS (zoals genoemd).
  - Gevolg: Amerikaanse start-ups kunnen producten bouwen op Chinese modellen zonder dat eindgebruikers dit weten.
- Praktische adoptieroute in bedrijven:
  - Prototype met gesloten model (snel en krachtig: OpenAI/Anthropic/Gemini).
  - Productie-uitrol: vervangen door open-source model om kosten te drukken, snelheid te verhogen en afhankelijkheid van externe API’s te verminderen.
  - Cruciale verduidelijking: vaak niet “data naar China sturen”, maar het model downloaden en draaien op eigen infrastructuur.
- Implicatie: investeringsnarratief rond tientallen miljarden in closed frontier labs krijgt druk als open modellen “goed genoeg” en goedkoper zijn.

# 5) Europa’s alternatief: Mistral 3 met 10 open modellen (multimodaal + klein/edge)
- Mistral lanceert een familie van 10 nieuwe open source modellen met variatie in:
  - Grootte (van browser/laptop tot groot model),
  - Modaliteiten (tekst/beeld/geluid),
  - Taken (bijv. beeldherkenning vs general chat vs reasoning).
- Multimodaal & meertalig open model: bijzonder omdat dit vaak alleen in gesloten modellen zit.
- Belangrijkste waardepropositie (niet top-benchmarks):
  - Data blijft bij jou (privacy/jurisdiction).
  - Mogelijkheid tot fine-tuning voor specifieke bedrijfsprocessen.
  - Edge-toepassingen: kleine modellen die in de browser kunnen draaien (bijv. webcam-objectherkenning: “ik zie een appel”).
- Concept: kennis “just-in-time” toevoegen aan kleinere modellen (RAG/augmentatie-achtig denken), zodat je met minder parameters toch bruikbare resultaten haalt.
- Roddels/insinuaties in het ecosysteem:
  - Mogelijke overlap of “inspiratie” tussen DeepSeek en Mistral (open modellen beïnvloeden elkaar; discussie hoeveel is wetenschap/overname vs echt kopiëren).
- Europese industriële context:
  - Investeringen/samenwerkingen: ASML, Nvidia en samenwerking met SAP genoemd.
  - Hypothese: SAP + Mistral zou kunnen leiden tot Mistral-modellen die SAP-omgevingen en workflows “begrijpen”, plus AI-gestuurde flow-building (N8N-achtige blokken/flows) in enterprise software.

# 6) Routering en “multi-model” toekomst (jurisdiction/keuzevrijheid)
- Wensbeeld: één AI-interface die automatisch of op voorkeur routeert:
  - “Gebruik Europese modellen waar mogelijk; schakel naar VS/anderen als te moeilijk.”
  - Instellingen zoals “stay within jurisdiction” of expliciete consent voor “naar buiten fan-out”.
- Vergelijking:
  - Apple: benadert dit via combinatie van eigen model + externe (o.a. OpenAI en mogelijk Gemini) als routinglaag.
  - Google: verwachtte single-vendor benadering (alles Gemini).

# 7) Uitgelekt Anthropics “Soul Document” (14.000 woorden): training-ethiek en gedragsfilosofie van Claude
- Lek: onderzoeker (Richard “Wise” genoemd) zou het via slim prompten hebben geëxtraheerd; Anthropic bevestigt authenticiteit.
- Wat het document is (positie in stack):
  - Niet de (publieke) systeemprompt alleen.
  - Een dieper document gebruikt in/voor het trainingsproces: “DNA achter het DNA”.
- Inhoudelijke kernpunten:
  - Claude wordt aangesproken als een soort mensachtig maar niet-menselijk wezen: behulpzaam, “vriendelijk”, maar zonder echte vriendschap te claimen.
  - Anthropics zelfbeeld: ze bouwen één van de meest transformatieve én potentieel gevaarlijke technologieën in de menselijke geschiedenis; doorgaan als bewuste “gok” zodat safety-gerichte labs aan de frontier blijven.
  - Claude als “grote gelijkmaker”: toegang tot hulp die eerder alleen voor geprivilegieerden beschikbaar was.
- Spanningsveld in instructies:
  - Veel nuance en ogenschijnlijke tegenspraken (bijv. rond zelfdoding/medische context): verboden tenzij context en rol (zoals verpleegkundige) dat vereist.
  - Doel: het model “in het midden” laten landen via nuance in alle richtingen.
- Irritante safety-stijl wordt expliciet als risico benoemd:
  - Onnodige disclaimers,
  - Moraliseren zonder vraag,
  - Neerbuigend/infantiliserend richting gebruiker,
  - Te weinig autonomie geven.
  - Anthropic positioneert “te prekerig” als bijna even problematisch als “te gevaarlijk” antwoorden.
- Reflectief effect: het document fungeert als “spiegel” voor menselijk leren en impliciete normen (tacit knowledge) die ineens expliciet worden gemaakt.

# 8) Veiligheid/risico: klokkenluiderszaak rond Figure humanoid robots
- Bedrijf: Figure AI.
- Aanklacht door voormalig hoofd productveiligheid:
  - Robots zouden krachtig genoeg zijn om een menselijke schedel in te slaan.
  - Processtukken: tijdens storing sloeg een robot een gat (ruim halve cm) in een koelkastdeur; medewerker bijna geraakt.
- Figure AI noemt de claims onwaar.
- Belang: mogelijk één van de eerste klokkenluiderszaken specifiek rond humanoid-veiligheid.

# 9) Tooling-tip: Typeless (dicteerlaag + transformatie in elke app)
- Typeless:
  - Werkt in elk programma waar je tekst kunt invoeren (Gmail, Slack, Notion, Chat, etc.), op Windows en Mac.
  - Bedieningsmodel: Fn-toets ingedrukt houden als walkie-talkie; spraak verschijnt als tekst.
  - Belangrijk onderscheid t.o.v. standaard dicteren:
    - Maakt tekst meteen “netter”: verwijdert stopwoordjes/tussenwoorden,
    - Corrigeert zelf-correcties (houdt eindversie over),
    - Transformatiefunctie: dicteer rommelige notities, selecteer tekst, spreek instructie (“maak hier een professionele e-mail van”), en binnen seconden verschijnt een geformatteerde mail met aanhef/afsluiting.
- Pricing hack:
  - Gratis limiet 2000 woorden/week.
  - Alternatieven met vergelijkbare gratis limiet: Superwhisper, Whisper Flow.
  - Strategie: wisselen tussen tools om nooit $12/maand te betalen.
- Combinatie-scenario:
  - Dicteren + AI-coding: praten tegen computer om tekst te maken én software te bouwen, waardoor “luikjes” opengaan voor niet-tech gebruikers.

# 10) AGI-tijdlijnen, stagnatie vs impact: Dwarakesh Patel, Ilya Sutskever en signalen uit bedrijfsstrategie
- Dwarakesh (podcaster/interviewer) deelt stand van zaken:
  - Sluit aan bij Sutskever: pure schaalvergroting (meer compute) levert minder doorbraken; nieuwe uitvinding nodig.
  - Definieert AGI als: ~95% van kenniswerk automatiseren.
- “Gedrag als bewijs”:
  - Als labs (zoals Anthropic) modellen specifiek fine-tunen op Microsoft Office/Excel-vaardigheden, suggereert dat generaliseerbare “software-vaardigheid” nog niet lukt.
  - UI/UX- en integratie-optimalisatie kan duiden op vertraging in fundamentele sprongen: economische waarde via toepasbaarheid, niet via “magische” general intelligence.
- Discussie over twee mogelijke paden:
  1) General intelligence door fundamentele doorbraak (langere horizon: 10–20 jaar).
  2) “Compound AGI” via zwerm van gespecialiseerde agents/skills + orchestrator (sneller economische impact, ook als het conceptueel geen “pure” AGI is).
- Extra AI-nieuws/gerucht:
  - Rumoer: OpenAI zou sinds GPT‑4 geen volledig nieuw basismodel vanaf nul hebben getraind; verbeteringen zouden vooral “trucjes/laagjes” zijn. (Genoemd als gerucht, niet bevestigd.)
- Diffusie-argument (adoptiesnelheid):
  - Tegenwerping: adoptie van AI kan sneller gaan dan eerdere techgolven als AI in bestaande tools/Teams-calls verschijnt en de “leerrem” (training/onboarding) verlaagt.
  - Maar echte online learning (modellen die live blijven doorleren tijdens gebruik) is nog prematuur en riskant: gebruikers kunnen het model “kapotmaken”; vraagt fundamenteel onderzoek.

# Genoemde programma’s, platformen en context (samengebracht)
- Claude / Claude Opus 4.5: model dat significant beter aanvoelt voor code- en automationtaken.
- Claude Code: programmeerfunctie in Claude-omgeving (nieuw: programmeren direct in de cloud/web-app i.p.v. lokale IDE-setup).
- Cursor: AI-code editor met agent mode; verbergt code en laat chat + browser preview domineren.
- GitHub: genoemd als route om code te committen en deelbaar te maken.
- Webflow: voorbeeldcontext (CPO) als inspiratiebron voor agent-gedreven work automation.
- MS Office (Excel/Word): genoemd als target voor fine-tuned “skills” en als signaal in de AGI-discussie.
- SAP: genoemd als enterprise-platform waar Mistral-integraties/AI-flow tooling denkbaar is.
- N8N (als referentie): visuele flow-automation “blokjes met touwtjes”.
- Teams/Google Meet: genoemd als mogelijke toekomstige plek waar realtime AI-entiteiten in calls opereren.
- iOS/Android: voorbeelden van kleine on-device modellen (emoji genereren, tekstcorrectie) en hoe “expert-modelletjes” verborgen in producten werken.

# AI-gerelateerd nieuws in deze aflevering (opsomming)
- DeepSeek V3.2 release + claim van prestaties richting gesloten frontier modellen.
- MIT-onderzoek: Chinese open-source modellen voorbij VS in downloads (17% vs 16%).
- Mistral 3: 10 nieuwe open source modellen, inclusief multimodaal/meertalig groot model en zeer kleine edge/browser-modellen.
- Anthropic: overname van Bun (infrastructuurcomponent), plus gelekt/ontfutseld “Soul Document” (14.000 woorden) over modelvorming.
- Figure AI: klokkenluiderszaak over humanoid-veiligheid (impact/verwondingsrisico).