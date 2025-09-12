# 112. GPT-NL is bijna klaar, maar zoekt nu klanten én daadkracht van de overheid (2025-08-06) [link](https://www.youtube.com/watch?v=U6Zypa22Wjs)


 # Hoofdthema en kern
Het gesprek gaat over GPTNL: een door TNO/een Nederlands consortium vanaf nul gebouwd groot taalmodel (Dutch + English) dat juridisch goed ingebedde, gelicentieerde data gebruikt en zich richt op professionele toepassingen (samenvatten, versimpelen, vraag‑antwoordsystemen). Belangrijke thema's: digitale soevereiniteit, rechtmatige dataverzameling en compensatie voor datamakers, technische opzet (pretraining + fine‑tuning), governance/financiering en adoptie bij overheden en bedrijfsleven.

# Belangrijkste feiten en status
- Initiële publieke investering: €13,5 miljoen.  
- Modelarchitectuur en grootte: ongeveer 26 miljard parameters.  
- Trainingsstrategie: volledig vanaf scratch (geen gebruik van bestaande foundation models zoals Mistral), met data waarvoor toestemming is gegeven of waarvoor licenties zijn afgesloten.  
- Compute: gehuurde capaciteit op de Nederlandse supercomputer Snellius (Surf) — dedicated cluster met 88 GPU’s (verdeeld over ~22 nodes) voor pretraining en experimenten.  
- Trainingsduur: pretraining duurt maanden (meerdere epochs), fine‑tuning en iteraties daarna. Eerste deadline/target: lancering voor launching customers rond 1 januari volgend jaar.  
- Doelprestatieniveau: inschatting rond GPT‑3 / GPT‑3.5 niveau qua algemene capaciteit, maar mogelijk beter voor specifieke Nederlandse taken (samenvatten/versimpelen).  
- Data & rechtmatigheid: nadruk op expliciete toestemming/licenties (grote Nederlandse nieuwsorganisaties en unieke datasets), geen massale ongevraagde scraping.  
- Verdienmodel/datacompensering: betaalde licenties voor professioneel gebruik; 50% van inkomsten wordt teruggeïnvesteerd/distributed naar dataeigenaren op basis van bijdrage en kwaliteit.  
- Teamgrootte: ~20–30 personen (kernteam + ingehuurde experts).

# Technische opzet en AI‑workflows
- Pretraining: trainen van basismodel vanaf nul op gelicentieerde en gecontroleerde datasets; meerdere maanden en meerdere epochs.  
- Instruction fine‑tuning: na pretraining wordt het model getraind op vraag‑antwoordparensets en instructies (samenvatten, versimpelen, opstellen e-mails, feitelijke vragen beantwoorden). Die trainingsdata worden door Nederlandse marktpartijen gegenereerd (niet crowdwork in Zuid‑Azië).  
- Preference tuning & safety: iteratieve voorkeurstraining (mensen beoordelen antwoorden), plus gebruik van modernere technieken zoals DPO (Direct Preference Optimization) als efficiëntere variant van klassieke RLHF. RLHF-achtige annotaties blijven onderdeel van het proces maar het team gebruikt recentere optimalisatietechnieken waar relevant.  
- System prompts & klant‑specifieke tuning: basislaag (neutrale/balans) + mogelijkheid tot domein‑of klantgebonden fine‑tuning en systeemprompts om gedrag (bijv. "conservatiever" voor bepaalde klanten) te sturen.  
- Data cleaning & augmentatie: voorafgaande rekenkracht nodig om data te filteren, cleanen, en mogelijk synthetische data of labels te genereren.  
- Deployment opties: model‑weights (als product) die integrators/partners in hun applicaties stoppen of model gehost als service/API (dan moet TNO/consortium operationeel beheer bieden). Let op: als ze ook de volledige applicatie leveren valt dat onder strengere AI Act‑verplichtingen.

# Use cases (gedetailleerd) en bijbehorende programma's/tools
Voor elk use case geef ik concreet welke onderdelen en programma's typisch betrokken zijn.

- Gemeentelijke / rijksoverheid — document‑samenvattingen & beleidsvoorbereiding  
  - Wat: automatische samenvattingen van beleidsdocumenten, versimpelen naar begrijpelijke taal, ondersteuning bij opstellen beleidsstukken, Q&A over lokale documenten.  
  - Combinatie van tools: GPTNL‑model (gefine‑tuned voor NL beleidsteksten) + document ingestion (DMS/SharePoint integratie) + OCR/processing voor gescande documenten + API of partner‑frontend (intranet/case‑management).  
  - Workflow: ingest → preprocessing → passage retrieval → instruction‑prompt (samenvatten/versimpelen) → kwaliteitscontrole + human in the loop.  
  - Waarom GPTNL: juridische duidelijkheid rondom data en betere Nederlandse contextkennis; minder privacy/AVG‑zorgen bij gebruik dan buitenlandse alternatieven.

- Telecom / customer contact centers — gespreksanalyse + automatisering  
  - Wat: transcripten analyseren, sentiment/CSAT meten, samenvatten gesprekken, automatisch antwoordvoorstellen, deels geautomatiseerde afhandeling (sluitende antwoorden op FAQ‑niveau).  
  - Combinatie van tools: ASR (spraak naar tekst; third‑party of lokale spraakmodule) + GPTNL voor samenvatting/entiteitsextractie + integratie met CRM/Genesys/CCaaS + analytics dashboard.  
  - Workflow: audio → ASR → transcript → GPTNL extracties (issues, intent, follow‑ups) → dashboard/automatische opvolging + menselijke controle bij kritische gevallen.

- Zorg / medische samenvattingen (voor administratieve ondersteuning)  
  - Wat: samenvatten van patiëntdossiers, hulp bij opstellen correspondentie, literatuuroverzicht voor professionals (niet medisch adviserend verdict geven).  
  - Combinatie van tools: veilige data‑connectors (EHR integratie) + GPTNL met strikte privacymaatregelen, logging en auditering, lokaal hosting of EU‑gehoste API + fine‑tuning op medische, maar geanonimiseerde datasets.  
  - Workflow: document retrieval → privacy‑scrub → GPTNL Q&A & samenvatting → clinician review.

- Educatie — lesmateriaal en uitleg in eenvoudig Nederlands  
  - Wat: versimpelen van vakteksten, opstellen oefenopgaven, gepersonaliseerde uitleg en samenvattingen voor leerlingen.  
  - Combinatie van tools: LMS integratie + GPTNL instructie‑tuning voor didactische taken + content management systeem voor leraren.  
  - Workflow: curriculumtekst → instructie prompt (leerdoel/wat vereenvoudigen) → output → docentcontrole & feedbackloop.

- MKB/commercie — knowledge base Q&A, workflow automations  
  - Wat: vragen beantwoorden uit bedrijfsdocumentatie (contracten, handleidingen), e‑mail drafts, interne knowledge assistants.  
  - Combinatie: GPTNL API/weights + connectors naar interne bronnen (SharePoint, Confluence) + partner‑gebouwde frontend (chatbot of Copilot‑achtige integratie).  
  - Workflow: document retrieval (RAG — retrieval augmented generation) → model antwoord → audit & logs → klantfeedback voor tuning.

# Nieuwe tools, methoden en workflows die genoemd zijn
- Direct Preference Optimization (DPO): genoemd als modernere methode om modelgedrag te sturen (sneller en efficiënter dan klassieke RLHF in sommige settings).  
- Instruction fine‑tuning / preference tuning: standaard pipeline na pretraining voor duidelijke taakinstructies en voorkeuren.  
- Gebruik van Snellius (Surf) als gehuurde supercompute voor pretraining en experimenten (dedicated cluster, niet gekocht).  
- Licentie‑first data‑workflow: vooraf toestemming vragen, licenties afsluiten met dataproviders (nieuwsmedia, mogelijk Koninklijke Bibliotheek en anderen) in plaats van ongevraagde scraping.  
- Revenue‑share mechanisme: 50% van GPTNL‑inkomsten terug naar dataeigenaren, met verdeelsleutel op basis van bijdragevolume en kwalitatieve weging.  
- Customer‑specific system prompt / fine‑tuning workflows: maatwerk per organisatie (bv. “conservatiever” of “progressiever”) via aanvullende fine‑tuning en systeemprompts.

# AI‑nieuws en beleidscontext in het gesprek
- Juridische discussies rond scraping en "fair use" (VS) en rechtszaken: verschillen tussen VS en Europa; Europa heeft geen brede fair use en meer focus op auteursrecht/AVG.  
- Controverses zoals Grok/X (Elon Musk) met ongepaste outputs en mogelijke juridische gevolgen; dit illustreert risico's van ongereguleerd uitrollen.  
- Europese en nationale aandacht: GPTNL wordt genoemd in Nederlandse nationale technologiestrategie en in partijprogramma’s (voorbeeld: VVD). Belang van digitale soevereiniteit.  
- Concurrentie en internationale initiatieven: andere Europese landen/consortia bouwen eigen LM’s; sommige projecten gebruikten data zonder toestemming wat relaties met data‑eigenaren onder druk zette.  
- Nextcloud en andere Europese spelers claimen soevereiniteitsoplossingen maar treffen schaal/engineeringslimieten; opschaling en ecosysteeminvesteringen zijn nodig.

# Governance, financiën en marktstrategie
- Governance: coöperatieve structuur met data‑providers aan tafel (niet enkel TNO‑besluitvorming). Transparantie en documentatie van datagebruik is prioriteit (AI Act compliance).  
- Verdienmodel: professionele licenties; prijsconformiteit (staatssteunregels) moet in acht worden genomen; mogelijke prijs indicatie in transcripties: vergelijkingen met Copilot (€30 → noemde €45).  
- Financiering: eerste tranche €13,5m; vervolgbehoefte voor significante volgende stap geschat op circa €10–15m (of kleine iteratieve rondes van €4–5m afhankelijk van doelen).  
- Markttoegang: focus op launching customers (rijksoverheid als ideële launching customer), maar ook telecom, zorg, educatie, banking/insurance. Mogelijke partners voor frontends en hosting; big tech heeft interesse maar zou soevereiniteitsrisico’s kunnen introduceren.

# Deploymentkeuzes en compliance (AI Act)
- Model alleen (weights) vs compleet AI‑systeem: als alleen weights geleverd worden blijft GPTNL in de rol van "AI component", maar zodra er een gebruikersinterface/operationalisatie komt valt het systeem onder de AI Act en vereist het strengere verantwoording, veiligheidstests en documentatie.  
- Compliance by design: GPTNL bouwt vanaf begin procedures voor verantwoording, documentatie, datatracering en veiligheidsmaatregelen in. Dit moet adoptiebarrières verminderen voor overheidsgebruik.  
- Hosting: voorkeur voor Europese/cloud‑partners of eigen hosting; praktische overwegingen (schaalbaarheid, security) maken het realistisch dat men met meerdere Europese cloud/hostingpartijen moet samenwerken.

# Risico's en open vragen
- Adoption gap: gemeenten en ziekenhuizen zijn traag met innovatie; procurement cycles en financiering (bijv. "ravijnjaar 2026") vormen risico voor vroege omzet en opschaling.  
- Financiering: vervolgfinanciering kritisch om model actueel en relevant te houden. Zonder doorlopende investeringen risico op achteruitgang.  
- Reputatierisico: fouten van een door overheid gesteund model kunnen groter publiek vertrouwen schaden; kritiek zal scherper zijn dan bij commercieel big tech.  
- Data governance: hoe fair en transparant wordt de 50% distributie uitgevoerd? Kwaliteitsmeting en bijdragecalculatie moeten technisch en bestuurlijk robuust zijn.  
- Opschaling hosting/integraties: Europees aanbod voor grootschalige, veilige hosting is beperkt; vereist samenwerking en investeringen in ecosysteem.

# Roadmap en volgende stappen
- Korte termijn: verdere pretraining (nog enkele epochs/releases), fine‑tuning (instruction + preference) en proof‑of‑concepts met partners (NFi, educatie, pilotgemeenten zoals Sittard‑Geleen). Target: eerste volledige modellen voor launching customers rond 1 januari.  
- Medium termijn: opschaling naar meer use cases, klantintegraties, verdere datasetacquisitie, opsporen van vervolgfinanciering (€4–15M scenario’s genoemd).  
- Lange termijn: groeien van ecosysteem (hosting, integrators, investeerders), mogelijk uitbreiden met spraak en meertaligheid, en samenwerken met andere Europese initiatieven.

# Conclusie / belangrijkste takeaway
GPTNL is een Nederlands initiatief dat kiest voor een juridisch en ethisch verantwoorde opbouw van een nationaal/neutraal groot taalmodel met sterke nadruk op Nederlandse data en soevereiniteit. Technisch is de aanpak traditioneel (pretrain → instruction fine‑tune → preference tuning/DPO), maar onderscheidend door toestemming/licenties, revenue‑sharing naar dataleveranciers en governance met stakeholders. Kernuitdagingen zijn opschaling (compute en hosting), adoptie door overheid/markt en vervolgfinanciering. Als deze knelpunten worden opgelost, kan GPTNL een relevante, veilige en Nederlandse optie worden voor professionele AI‑toepassingen.