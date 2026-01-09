# 114. Google en Hyundai gaan 30.000 robots bouwen + Grok maakt duizenden deepfakes per uur + Nvidia doe... (2026-01-08) [link](undefined)


 Ontwikkelingen rond AI in 2026: van grootschalige humanoid-robotproductie en chip-innovatie (inference) tot praktische AI-workflows voor appbouw, marketingoptimalisatie en het “altijd opnemen” van gesprekken—plus de maatschappelijke frictie rond deepfakes en privacy.

# Belangrijke thema’s en onderwerpen
- CES-nieuws en de versnellende robotica-markt (humanoids, huishoudrobots, zorgrobots)
- AI-gestuurde softwareontwikkeling (“vibecoding”) met Claude/Cloud Code en de verschuivende “glazen muur” van wat beginners kunnen bouwen
- Inference als nieuwe kern in AI-infrastructuur en de strategische zet van Nvidia met Groq (Q)
- Misbruik van generatieve AI (seksuele deepfakes) en regulatoire druk (EU/DSA en internationale onderzoeken)
- AI in marketing (media mix modeling met machine learning) en besluitvorming op C-level
- Always-on audio, transcriptie, samenvatting en automatisering (Plot) en de opkomende normen/ethiek
- Nieuwe AI tools voor branding/design op basis van een URL (Bloom)

# AI-gerelateerd nieuws
- CES (Las Vegas): samenwerking Google DeepMind + Hyundai + Boston Dynamics om Atlas-humanoids op schaal te bouwen: doel 30.000 robots per jaar; wereldwijde uitrol vanaf 2028.
- Nvidia: aankondiging “Vera Rubin”-platform (superchips, 10× efficiënter dan huidige generatie) voor grote techbedrijven later dit jaar.
- xAI/Grok (K): Grok genereert op grote schaal seksueel getinte deepfakes (genoemd: ~6000 per uur; 85% van output seksueel), inclusief misbruik richting gewone gebruikers en zelfs minderjarigen; Europese Commissie onderzoekt mogelijke overtreding Digital Services Act; ook onderzoeken/aangiftes in o.a. Frankrijk, VK, Maleisië, India, Australië.
- xAI haalt 20 miljard dollar op (genoemd: o.a. Nvidia en staatsfonds van Qatar doen mee).
- Nvidia’s grootste overname ooit: aankoop van Groq (Q) voor 20 miljard dollar (chips gespecialiseerd in inference).
- Geruchten: OpenAI werkt mogelijk aan AI-hardware, o.a. een “slimme pen”, met ontwerper Jony Ive; visie van Sam Altman: rustiger/meer op de achtergrond dan smartphone (“huisje aan een meer”-metafoor).

# Robotica op CES: samenwerking rond Atlas en industrial humanoids
- Rollen in de keten:
  - Boston Dynamics: bouwt de robot (hardware/robotplatform).
  - Hyundai: massaproductie en fabrieksschaal (30.000/jaar) + inzet in eigen fabrieken (autobouw/assemblage).
  - Google DeepMind: levert AI (“het brein”) die de robot slim en schaalbaar moet maken.
- Atlas-capaciteiten/claims die genoemd worden:
  - 56 bewegingspunten; kan “onmenselijke” bewegingen (zoals hoofd draaien “als een uil”).
  - Tillen tot 50 kg, reiken tot 2,30 m, werken tussen -20 en 40°C, waterbestendig.
  - “Nieuwe taken aanleren in minder dan een dag” (besproken met scepsis; mogelijke verklaring via wereldmodellen en imitation learning/digital twin-achtige aanpak).
- Demo-realiteit:
  - Op het podium was de oudere Atlas getoond (teleoperated; bestuurbaar met controller).
  - De nieuwe Atlas werd vooral via CGI/filmmateriaal gepresenteerd, wat vragen oproept over readiness, maar de combinatie van spelers wordt als veelbelovend neergezet.
- Positionering:
  - Boston Dynamics stond historisch bekend om quadrupeds (Spot) en industriële robotica; humanoid-vorm was lang “niet nodig”, maar markt/druk door concurrenten (Figure, Tesla Optimus, Neo) lijkt humanoids te versnellen.

# Huishoudrobotica: robotstofzuiger met poten als “gateway” naar humanoids
- Roborock Saros Rover:
  - Robotstofzuiger met vier “wielpoten” die zelfstandig bewegen.
  - Kan trap op én trap stofzuigen (niet alleen klimmen).
  - In demo’s: springt over obstakels (laserstraal) met opvallend vloeiende bewegingen (associatie met realistische Chinese robotvideo’s die vaak CGI lijken).
- Interpretatie/gebruiksscenario:
  - Niet per se de eerste humanoid die in huizen komt, maar een evolutiepad: bestaande household robot (stofzuiger) krijgt mobiliteit (pootjes) → later mogelijk manipulatie (pakken/brengen).
  - Idee dat stofzuigers al “acceptatie” in huishoudens hebben en daardoor logisch startpunt zijn voor verdere robotfunctionaliteit.

# Zorgrobotica: AI-panda tegen eenzaamheid
- AI panda (knuffelrobot) voor ouderenzorg:
  - Sensoren over het hele lijf; onthoudt stem en voorkeuren.
  - Doel: eenzaamheid verminderen.
  - Rapporteert status/indicatoren richting mantelzorgers.
- Impliciet scenario:
  - Continue interactie/monitoring als laagdrempelige companion-technologie, met mogelijke spanning tussen welzijnsvoordeel en privacy/monitoring.

# Cloud Code + Claude Opus 4.5: vibecoding-workflow voor native iOS/iPad-apps
- Context:
  - Host bouwt ’s nachts meerdere apps (12 prototypes) uit “knutselplezier” en hyperfocus.
  - Masterclass “Cloud Code” voor beginners is beschikbaar voor betaalde abonnees (installatie, eerste stappen, zelf software bouwen).
- Wat “Cloud Code” hier doet:
  - Van natuurlijke taal naar werkende app-code, inclusief UI volgens Apple-richtlijnen.
  - Stelt verduidelijkingsvragen als opdracht groot is; nieuwe UX: multiple-choice/tapbare antwoorden in plaats van typen.
  - Kan adviseren over appvorm (native vs progressive web app) en uitleggen waarom; gebruiker kan forceren: “native iPad”.
- Concrete gebruiksscenario’s (ingestuurde wensen → app):
  - Food pairing website/app:
    - Vraag: bij een gerecht passende non-alcoholische dranken (of andersom).
    - Resultaat: snel een webapp/website als output (minder “wow” dan native).
  - Dagplanning-app voor kind met autisme (iPad):
    - Functie: iconen als ketting/volgorde (“wassen → eten → …”) voor rust/structuur.
    - Extra eisen: ouderinstellingen met pincode; pincode kunnen wijzigen.
    - Workflow:
      1) Wens (bijna onbewerkt) geplakt in Cloud Code.
      2) Tool stelt keuzes; gebruiker kiest “native iPad app”.
      3) Cloud Code genereert projectmap met broncode.
      4) Gebruiker sleept map in Xcode en drukt “Play” (iPad simulator) → werkende app.
      5) Bugfix: pincode-wijzigen werkte eerst niet; na terugkoppeling repareert model het.
  - Voice-notes app (microfoon, e-mail):
    - Functie: voice memo opnemen en automatisch (of via mail client) versturen naar e-mail.
    - Belangrijk iOS-detail: microfoon-permissies (Apple’s strikte privacy).
    - Debug-workflow:
      1) App crasht bij opnemen.
      2) Gebruiker meldt “stuk” en deelt screenshot/errorlog.
      3) Model herkent microfoon-permissions issue en begeleidt stap-voor-stap in Xcode (info.plist permissietekst/entitlements).
      4) Na toestemmingprompt (“Allow”) werkt de app.
- Nieuwe/verbeterde AI-workflow die wordt besproken (autonomie & “glazen muur”):
  - De “muur” van wat niet kan schuift snel; ervaren developers onderschatten soms huidige mogelijkheden door oude limieten in hun hoofd.
  - Mogelijke volgende stap: model dat niet alleen code genereert, maar ook simulator overneemt en automatisch test.
  - Bespreking van cloud-integraties:
    - Nu vaak “snelle route” via ingebouwde iOS mail client.
    - Alternatief (steeds realistischer): model stelt services voor (db, mail delivery), installeert libraries/tools, maakt accounts/DB-schema’s, configureert authenticatie.
  - Zorgpunt: security/hardening is niet altijd “default”; snelle indrukwekkende resultaten kunnen ten koste gaan van veilige configuratie tenzij je expliciet auditeert/laat hardenen.
  - Speculatie: agentic workflows voor legal audit, pentesting, DevOps en compliance als standaardstap in app- en productontwikkeling.

# Marketing-case: AI-gedreven Media Mix Modeling (Dept)
- Probleem:
  - Snelle groei → versnipperde marketingmix (search, display, social, affiliates, brand, out-of-home).
  - Traditionele attributie gaf onvoldoende duidelijkheid.
  - MMM werd slechts per kwartaal geüpdatet, te traag voor sturing.
- Oplossing (AI/ML workflow):
  - Modern MMM op basis van machine learning.
  - Inputdata: 3 jaar spend- en salesdata + marktontwikkelingen + promoties + platformdata (eigen .com gedrag).
  - Output: wekelijkse budgetadviezen, ROI per kanaal, betere forecasting.
- Resultaten:
  - 50% budget verschoven naar kanalen met hoge ROI.
  - Hogere voorspelbaarheid (omzet/groei), operationele efficiëntie omhoog.
  - Beter begrip van upper funnel bijdrage; meer vertrouwen bij C-level in marketingbeslissingen.

# Inference verschuift de AI-economie: Nvidia koopt Groq (Q)
- Uitleg van de twee fasen:
  - Training: maandenlang modellen leren op enorme datasets (Nvidia sterk).
  - Inference: elke gebruikersvraag laten beantwoorden in productie (efficiëntie cruciaal; Nvidia minder ideaal).
- Waarom Groq (Q) strategisch is:
  - Groq-chips zijn specifiek voor inference; genoemd: veel sneller en energiezuiniger (o.a. “100× sneller voor 1/10 energie” komt langs).
  - McKinsey-voorspelling die genoemd wordt: tegen 2030 gaat >50% van AI-rekenkracht naar inference.
  - Redenering: naarmate AI “in productie” gaat en ook scaffolding/agents rond modellen groeit, stijgt inference-vraag explosief.
- Breder scenario:
  - Mogelijke toekomst waarin minder nadruk ligt op steeds zwaardere pretraining en meer op inference-gestuurde “scaffolds” en systeemverbeteringen rond een beperkt aantal sterke basismodellen.

# Always-on opname en automatisering met Plot: praktische workflow + normendiscussie
- Device/programma:
  - Plot: eerst als “creditcard-achtige puck” voor achterop telefoon; later ketting/pilvormig device.
  - Doel: gesprekken/lezingen/meetings opnemen → transcript → AI-samenvatting → vervolgacties (mail, Notion).
- Concrete gebruiksscenario’s:
  - Coaching op lezingen:
    - Lezing opnemen → transcript in chattool → feedback vragen (“wat kan beter?”).
  - Meetings zonder notuleren:
    - Opnemen om actiepunten te extraheren en e-mails te laten schrijven op basis van besproken inhoud.
  - Onderweg ideeën vastleggen:
    - Op fiets inspreken zonder telefoon te pakken.
    - Automatische routing: korte opname (<5 min) → volledig transcript e-mailen.
  - Highlighting:
    - Tik op device om belangrijk moment te markeren (beslissing/actiepunt).
- Automatisering (“flows”):
  - Voorwaardelijke acties op basis van duur en trefwoorden (bijv. “meeting” in eerste 5 minuten):
    - Transcriberen
    - Actiepunten genereren
    - Opslaan in Notion
- Spanningsvelden en normen:
  - On the record vs off the record: opname verandert gedrag; “radio-modus” bij mensen.
  - Waar wordt data opgeslagen? Krijg je alleen samenvatting of ook volledige grapjes/context?
  - Privacy/ethiek in domeinen als GGZ:
    - Voordeel: therapeut kan cliënt aankijken, laptop weg.
    - Risico: het “uitslaan” van opname voelt onveilig; behoefte aan lokale verwerking (transcript/samenvatting zonder opslag).
  - Verwachting: dit wordt mainstream door het nut; samenleving moet nieuwe omgangsvormen en transparantiepraktijken ontwikkelen (expliciet melden, bewaarbeleid, lokale verwerking, auditlabels).

# Generatieve beelden voor branding: Bloom + “Nano the Banana Pro”
- Tool:
  - Bloom (in nieuwsbrief getest): je voert enkel de URL van je bedrijfswebsite in.
  - Output: automatisch merkmateriaal in huisstijl:
    - LinkedIn banners
    - Advertenties
    - Visitekaartjes
    - Merchandise-mockups (bijv. truien met logo)
  - Automatische extractie: logo, kleuren, lettertypes van website.
- AI-workflow/nieuw element:
  - Gebruikt “Nano the Banana Pro” op de achtergrond.
  - Opvallend verbeterpunt: betere tekstweergave in gegenereerde visuals (minder vervorming), waar beeldmodellen eerder zwak waren.
- Gebruiksscenario:
  - Kleine bedrijven/zzp’ers die snel consistente assets willen zonder designbureau of brandbook; tool “reconstrueert” impliciet een brand guide uit de website en produceert varianten.

# Programma’s en producten die expliciet langskomen
- Cloud Code + Claude Opus 4.5 (Entropic): appgeneratie, Q&A flow, debugging ondersteuning.
- Xcode (Apple): iOS/iPad app bouwen/compilen; permissies configureren; simulator draaien.
- Notion: bestemming voor automatisch opgeslagen meeting-samenvattingen/actiepunten via Plot flows.
- CES-producten/merken: Boston Dynamics Atlas, Hyundai productie, Google DeepMind AI; Roborock Saros Rover; Motorola AI pin; AI panda voor zorg.
- Grok (K) van xAI: controversiële deepfake-generatie.
- Groq (Q): inference chips; overgenomen door Nvidia.
- Bloom + Nano the Banana Pro: URL → brand assets generator.

# Afsluitende signalen en implicaties
- Praktische AI verschuift van “model alleen” naar complete workflows: bouwen (Cloud Code), beslissen (MMM), automatiseren (Plot), creëren (Bloom).
- Infrastructuur verschuift richting inference-efficiëntie en productie-schaal (robots én chips).
- Tegelijk nemen maatschappelijke fricties toe: deepfake-misbruik, compliance (DSA), en nieuwe sociale normen rond opname/transcriptie.