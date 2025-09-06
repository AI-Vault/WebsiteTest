# 90. Why Satya Nadella Believes AI Will Create More Jobs, Not Destroy Them | AI Report
Views: undefined (2025-06-19) [link](undefined)


 # Belangrijke onderwerpen en thema’s
- Toekomstige werkverdeling: massale verschuivingen in taken en vaardigheden binnen 5 jaar; drudgery wegautomatiseren; verschuiving naar hogere abstractie (werken als architect/overzien van agents).
- AI als alledaags gereedschap: diffusie van AI zoals vroeger Excel; brede toegankelijkheid versus concentratie bij techbedrijven.
- Agents en coderingsworkflows: evolutie van code-completions naar multi-agent, branch-PR- en review-workflows.
- Sector-specifieke adoptie: voorbeelden uit gezondheidszorg, juridisch werk en financiële dienstverlening.
- Hardware en platformshifts: mogelijkheid dat Microsoft het kenmerkende hardwareproduct voor AI creëert.
- Vergelijking van modelseries: Phi-serie (Anthropic) versus GPT-4o; verwachting dat sommige modellen tegenwoordig vergelijkbaar krachtig zijn.
- Governance, aansprakelijkheid en veiligheidschecks: noodzaak van maatschappelijke checks en regels bij grootschalige deployment; legale limitering van autonome AI-uitvoer.
- Risico’s en ongewenste toepassingen: cybercriminaliteit, biosecurity en andere onbedoelde gevolgen naast voordelen.
- Onderwijs en persoonlijke ontwikkeling: gepersonaliseerde tutors en vroegtijdige leerhelpen voor kinderen.

# Gebruiksscenario’s en gebruikte programma’s (gedetailleerd)
- Ziekenhuisdischarge automatiseren
  - Programma/stack: EMR-systeem (voorbeeld ChipSoft) + open data-laag gekoppeld aan een LLM.
  - Workflow: EMR opent data-tier → LLM krijgt gestructureerde gegevens en prompt → LLM genereert volledige ontslagbrief/administratie → arts controleert en valideert → output in EMR opgeslagen en verzonden.
  - Voordelen: tijdsbesparing voor verpleegkundigen/artsen, lagere administratieve kosten, snellere ontslagprocessen.

- Paralegal-documentverwerking in advocatenkantoren
  - Programma/stack: Copilot Studio (of gelijkaardige agent-omgeving) + documentopslag/EDR.
  - Workflow: paralegal bouwt agents in Copilot Studio die documenten scannen, samenvatten, relevante clausules vinden en checklists invullen; agent reduceert repetitieve taken; mens valideert en finetunet.
  - Voordelen: vermindering van weekendwerk, afname van monotonie, hogere productiviteit en job-kwaliteitsverbetering.

- Softwareontwikkeling met multi-agent coding workflow
  - Programma/stack: GitHub Copilot (code-completion), Copilot/agents (agent mode), versiebeheer (Git), CI/CD pipeline.
  - Stappen:
    1. Copilot gebruikt voor in-flow code-completions en als zoekassistent.
    2. Agent-mode: agents uitvoeren multi-file edits op basis van taakomschrijving.
    3. Coding agent maakt eigen branch en genereert een Pull Request (PR) met implementatie.
    4. Code-review agent voert automatische review/tests uit en geeft feedback of wijst terug naar ontwikkelaar.
    5. Menselijke software-architect of engineer valideert, attesteert en merge-take beslissingen.
  - Voordelen: versnelling van ontwikkelcycli, schaalbare orkestratie van taken, menselijke rol evolueert naar architect/validator.

- Fintech en financiële dienstverlening: gepersonaliseerde producten en grotere productiviteitsoutput
  - Programma/stack: bank core systems + AI-agents, data lakes, klant-UI.
  - Workflow: kenniswerkers gebruiken AI om analyses, productproposities en personalisatie te maken; hogere productiviteit leidt tot meer aanbod en financiële inclusie.
  - Voordelen: meer producten, potentieel hogere GDP-output, betere personalisatie.

- Onderwijs en gepersonaliseerde tutoring
  - Programma/stack: adaptive LLM-based tutors, interactieve visualisaties (JS/3D renders), gepersonaliseerde prompts.
  - Workflow: leerling vraagt uitleg → LLM geeft empathische, op leervoorkeur afgestemde uitleg + interactieve visualisaties → leerling oefent met gepersonaliseerde opdrachten.
  - Voordelen: lagere drempel voor complex begrip, snellere inhaalslagen en levenslang leren.

# Nieuwe tools en AI-workflows (in detail)
- Copilot Studio
  - Omschrijving: omgeving om agents te bouwen en te orkestreren voor domeinspecifieke taken (documentanalyse, automatisering van workflows).
  - Belangrijkste functies: low-code/no-code agent-creatie, integratie met bedrijfsdata, mogelijkheid tot het samenstellen van multi-agent pipelines.
  - Gebruik: door niet-technische gebruikers (bijv. paralegals) om repetitieve taken te automatiseren.

- Coding agents / Agent mode in ontwikkelflows
  - Omschrijving: agents die op taakniveau werken (issue → branch → implementatie → PR), zelfstandig multi-file wijzigingen doorvoeren en tests draaien.
  - Integratiepunten: versiebeheer (branching), CI pipelines, code review agents.
  - Rol van de mens: architectuur-overzicht, juridische aansprakelijkheid, finale validatie en attesten.

- Code review agent
  - Omschrijving: agent die automatisch PR’s beoordeelt op stijl, veiligheid, testen en regressie-risico’s; kan ook voorgestelde fixes genereren.
  - Belang: verhoogt kwaliteit en snelheid, maar menselijke verantwoordelijkheid blijft cruciaal voor aansprakelijkheid.

- Openen van EMR-data-tier naar LLM-tier
  - Omschrijving: architectuurpatroon waarbij gestructureerde EMR-data beschikbaar wordt gesteld aan LLMs via veilige toegangslag.
  - Noodzakelijke veiligheidsmaatregelen: toegangscontrole, auditing, prompt-sanitatie, model- en output-validatie.

- Rollenherontwerp (voorbeeld LinkedIn full stack functie)
  - Omschrijving: samensmelten van verschillende functies tot nieuwe rollen (bijv. product manager + designer + front-end engineer → “full stack developer”).
  - Effect: vergroot arbeidskrachtenpool en herijkt welke skills waardevol zijn in AI-augmented workflows.

# Arbeidsmarkt, vaardigheden en maatschappelijke aanbevelingen
- Vaardigheidsverschuiving: routine-expertise wordt gecommoditiseerd; belang van abstracte vaardigheden (architectuur, supervisie, verificatie, menselijke interactie).
- Productiviteit vs werkvolume: productiviteit kan stijgen; output kan toenemen waardoor nieuwe producten en diensten ontstaan; arbeidsvraag verandert, niet per se gelijk massale werkloosheid.
- Opleiding en lifelong learning: aanbeveling voor beleidsmakers en bedrijven om technologie te diffusiëren en werknemers om te scholen naar hogere abstractieniveaus.
- Governance-aanpak: implementatie van safety checks en maatschappelijke toestemming (social license) voor brede deployment van frontier modellen.

# Risico’s, aansprakelijkheid en veiligheidsmaatregelen
- Juridische en aansprakelijkheidsrestricties vormen fundamentele limiterende factoren voor autonome AI-toepassingen.
- Onbedoelde gevolgen: misbruik door cybercriminelen, biosecurity-risico’s en andere kwaadwillige toepassingen.
- Beheersmaatregelen: multilayer safety checks, helderheid over sociale permissie, transparantie en monitoring bij brede deployment.

# AI-gerelateerd nieuws en actuele claims uit het gesprek
- Phi-series (Anthropic) worden genoemd als vandaag al meer of minder even krachtig als GPT-4o — claim dat sommige modellen vergelijkbare capaciteiten hebben.
- Microsoft ambities: mogelijk ontwikkelen van een defining hardware form factor voor AI; streven naar wereldmodellen die krachtig genoeg zijn voor zelfrijdende toepassingen.
- ChipSoft (EMR-leverancier) heeft data-tier geopend voor LLM-integratie in ziekenhuizen (voorbeeld UMC Utrecht -> praktijkcase).
- Interne productideeën (LinkedIn) en voorbeelden van Copilot/Copilot Studio adoptie in praktijk (paralegal use case, coding agents) dienen als actuele signalen van productimplementatie.

# Conclusieve observaties (korte samenvatting van de visie)
- Korte termijn (vijf jaar): sterke versnelling in adoptie; veel kenniswerk wordt heringedeeld naar hogere-abstractie-rollen waarbij AI drudgery vermindert en productiviteit stijgt.
- Langere termijn: onzekerheden blijven (risico’s, juridische kaders), maar met adequate governance en brede diffusie kunnen maatschappelijke voordelen (gezondheidszorg-efficiëntie, onderwijs, financiële inclusie) substantieel zijn.
- Menselijke rol verschuift van uitvoerder naar architect, validator en waardetoevoeger van menselijke kwaliteiten (bijv. empathie, zorg), met blijvende noodzaak tot toezicht en aansprakelijkheid.