# 90. Why Satya Nadella Believes AI Will Create More Jobs, Not Destroy Them | AI Report
Views: undefined (2025-06-19) [link](undefined)


 De transformatie van kenniswerk en arbeidsmarkten door AI binnen vijf jaar (2029): voorspellingen, concrete use‑cases, benodigde beleidsmaatregelen en de rol van tools zoals Copilot, coding agents en LLM-integraties in bestaande systemen.

# Belangrijkste thema's
- Voorspellingen voor 2029: welke AI‑mogelijkheden wel/geen realiteit worden (avataarsimulaties, 12‑jarigen als programmeurs, jobverschuivingen, hardware‑leadership, modelvergelijkingen).
- Commoditisering van huidige expertise en ontstaan van nieuwe expertises.
- Diffusie en democratisering van AI (vergelijking met Excel‑adoptie).
- Reductie van routinematig, administratief werk (drudgery) in sectoren als gezondheidszorg en juridisch werk.
- Nieuwe rollen: mensen als architecten, toezichthouders, testers en attestators in workflows met meerdere AI‑agents.
- Juridische en aansprakelijkheidsbeperkingen als rem op volledige vervanging van mensen.
- Onderwijs en persoonlijke tutoring via empathische AI.
- Risico's en benodigde maatschappelijke/beleidsmatige checks (cybercriminaliteit, biosecurity, veiligheidschecks).

# Concrete gebruiksscenario's en gebruikte programma's (gedetailleerd)
- Ziekenhuis (discharge papers)
  - Gebruikte systemen: EMR/EPD (voorbeeld: ChipSoft), LLM‑laag gekoppeld aan data‑tier.
  - Workflow:
    1. EMR opent een patiëntdossier en stelt relevante data (metingen, diagnoses, behandelingsnotities) beschikbaar.
    2. Een prompt of template naar het LLM: instructie om ontslagbrief / discharge summary te genereren met medische kernpunten en nazorginstructies.
    3. LLM genereert conceptdocument en vult formulieren volgens lokale standaarden.
    4. Menselijke arts of verpleegkundige reviewt, corrigeert en ondertekent (verzekert aansprakelijkheid).
    5. Definitieve ontslagbrief wordt opgenomen in het EPD en uitgegeven aan patiënt.
  - Resultaat: grote tijdsbesparing, minder administratieve belasting, meer tijd voor directe patiëntenzorg.

- Juridisch/Paralegal (M&A documentreview)
  - Gebruikte tools: Copilot Studio (agentbouw), LLMs voor documentanalyse.
  - Workflow:
    1. Upload grote datasets contracten/overeenkomsten naar de tool.
    2. Agents zijn geconfigureerd om te taggen, samenvatten, clausules te extraheren en risico's te markeren.
    3. Agent genereert checklist/issue‑lijst voor menselijke review.
    4. Paralegal superviseert, past prompts of agentconfiguraties aan en valideert output.
  - Resultaat: drastische reductie van repetitieve weekendwerk; paralegal “wil gered worden van haar baan” = wil bevrijd worden van routinetaken.

- Softwareontwikkeling (ontwikkelingsagenten en Copilot)
  - Gebruikte tools: GitHub Copilot, Copilot in‑flow features, Copilot Studio/agent modes, coding agents, code‑review agents, versiebeheersysteem (git).
  - Workflow (evolutie van taken):
    1. Code completion/in‑flow assistance: ontwikkelaar ontvangt snippet‑aanvullingen tijdens programmeren.
    2. Agent‑modus: agent voert multi‑file edits uit op basis van kleine taken (refactors, consistente naming, eenvoudige features).
    3. Coding agent (volledige feature): krijgt issue/taak, maakt een feature branch, implementeert code, runt tests, genereert PR (pull request).
    4. Code‑review agent: voert statische checks, style/architectuurregels en veiligheidschecks uit en levert reviewfeedback.
    5. Menselijke softwarearchitect of senior ontwikkelaar verifieert ontwerpkeuzes, security/liable aspecten en merge/attestatie.
  - Resultaat: ontwikkelaars schuiven naar architect- en coördinatiefuncties; meer abstractieniveau en agent‑orchestratie.

- Productontwikkeling / LinkedIn voorbeeld (herdefiniëring rollen)
  - Gebruikte programma's: interne product tooling, Copilot‑achtige hulpmiddelen.
  - Concept: creëer nieuwe functietypen (bijv. “full‑stack developer” die productmanagement, design en front‑end combineert) met AI‑assistentie om kleine teamrollen te synthetiseren.
  - Resultaat: vergroot arbeidsmarkt door mensen productiever te maken met gecombineerde taken.

- Onderwijs / Persoonlijke tutoring
  - Gebruikte tools: empathische, gepersonaliseerde LLM‑tutoren (Copilot‑achtige interfaces).
  - Workflow:
    1. Learner stelt vragen of volgt interactieve simulaties (bijv. visualisatie van Maxwell‑vergelijkingen).
    2. LLM past uitlegstijl aan leerstijl (visueel, stap‑voor‑stap) en gebruikt interactieve voorbeelden of code‑simulaties.
    3. Feedbackloops en aangepaste oefenopdrachten verbeteren begrip.
  - Resultaat: lagere drempel voor complexe concepten; gepersonaliseerd leren vanaf jonge leeftijd.

# Nieuwe tools en AI‑workflows (gedetailleerd)
- Copilot (algemeen)
  - Functie: contextuele code/schrijfassistent, in‑flow ondersteuning.
  - Input/Output: code, comments of nattaalprompt → suggesties, code snippets.
  - Limitaties/opmerkingen: goed voor productiviteit, maar menselijke verificatie vereist.

- Copilot Studio / Agent‑bouwplatform
  - Functie: gebruikers (ook niet‑engineers) kunnen gespecialiseerde agents bouwen voor workflowautomatisering.
  - Hoe het werkt:
    - Gebruiker definieert taken, data‑connectors en instructies/prompts.
    - Studio instelt agents die documenten verwerken, queries uitvoeren, acties ondernemen (bv. genereren van documenten).
    - Agents kunnen georchestreerd worden in pipelines met menselijke in‑the‑loop controles.
  - Use cases: paralegals die automatisering bouwen, teams die interne procesautomatisering maken.

- Coding agents / Agent mode in ontwikkeltooling
  - Functie: autonoomere AI‑agents die grotere code‑taken uitvoeren (multi‑file, branch, PR).
  - Workflow details:
    - Ontvangen van issue/taak + repository context.
    - Lokale uitvoering: code genereren, tests (unit/integratie) draaien, statische checks uitvoeren.
    - Creëren van feature branch en PR met changelog/commit messages.
    - Interactie met code‑review agent of menselijke reviewer.
  - Belang: verschuift rol van ontwikkelaar naar ontwerper/architect/validator.

- LLM‑integratie met EPD/EMR systemen
  - Functie: directe koppeling tussen medische data‑lagen en LLM‑laag voor documentgeneratie en summarizing.
  - Veiligheidsmechanismen aanbevolen: toegangscontrole, auditing, logging, menselijke attestatie en standaardisatie van prompts/templates.

- Code‑review agents
  - Functie: automatisch reviewen van PRs op stijl, veiligheid, regressies en architecturele consistentie.
  - Rol: eerstelijns kwaliteitscontrole; output ter verificatie door menselijke reviewers.

# AI‑gerelateerd nieuws en claims uit de tekst
- Voorspellingen 2029 (kort):
  - Teams‑meeting met AI‑avatar ononderscheidbaar van echte persoon? Antwoord: Nee.
  - 12‑jarigen met AI zullen huidige professionele programmeurs overtreffen? Antwoord: Ja.
  - Meer dan 25% van westerse kantoormedewerkers heeft tegen 2029 een sterk verschillend werk? Antwoord: Ja.
  - Microsoft zal het definiërende hardware‑formaat voor AI maken? Antwoord: “I hope so” (niet hard bevestigd).
  - Phi‑series modellen even krachtig als GPT‑4o? Claim: “They are today, more or less.” (vergelijking, impliciete claim van comparable capability).
  - Microsoft zal wereldmodellen ontwikkelen die krachtig genoeg zijn voor self‑driving? Antwoord: “I hope so.”
- Concrete initiatieven/demos genoemd:
  - Demonstratie bij keynote: koppeling EMR → LLM voor ontslagbrieven (voorbeeld UMC Utrecht + ChipSoft).
  - Paralegal in VK gebruikte Copilot Studio om haar eigen agents te bouwen en werk te verminderen.
  - LinkedIn experimenteert met functieredesign (full‑stack rol) ondersteund door AI.
- Belangrijk nieuwswaardepunt: nadruk dat krachtige modellen al beschikbaar en bruikbaar zijn in werkprocessen; oproep tot maatschappelijke checks.

# Beleids-, ethische- en veiligheidsaspecten
- Aanbeveling: diffuseer technologie breed — maak AI net zo alledaags bruikbaar als Excel geweest is.
- Noodzaak voor meerdere checks bij deployment van frontier models:
  - Veiligheidschecks (technisch).
  - Maatschappelijke checks (sociale toestemming, publieke nut).
  - Regelgeving rond aansprakelijkheid en menselijke attestatie.
- Risico's genoemd: cybercriminaliteit, biosecurity, onbedoelde maatschappelijke effecten.
- Sociaal beleid: voorbereiding van arbeidsmarkttransities, om‑/bijscholing en het waarderen van nieuwe menselijke eigenschappen (bijv. empathie, menselijke aanraking).

# Conclusies en implicaties
- Korte termijn (binnen 5 jaar): substantiële verandering in hoe kenniswerk wordt uitgevoerd—AI zal drudgery wegnemen en werkprocessen herconfigureren; ontwikkelaars en andere professionals worden meer architecten/validatoren.
- Langere termijn: productiviteitsstijging kan economische output verhogen maar vereist beleid voor omscholing en wettelijke kaders om risico's te mitigeren.
- Praktisch advies uit de tekst: maak AI‑tools breed beschikbaar, ontwerp workflows met menselijke verificatie, en implementeer veiligheids‑ en maatschappelijke toetsing voordat modellen breed worden ingezet.