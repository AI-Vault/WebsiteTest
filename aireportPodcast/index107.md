# 107. GPT 5.1 is een sycofant + Chinees model verslaat ChatGPT en is gratis + photoshoppen door te praten (2025-11-13) [link](undefined)


 Snelle versnelling in AI-capabilities en AI-toepassingen: nieuwe modelrelease(s) (GPT‑5.1), opkomst van sterke (open) Chinese modellen (Kimi/K2), AI-beeldbewerking “via tekst” in consumentenapps (Google Foto’s), plus praktische implicaties voor media, bedrijven en productstrategieën (scaffolding/“waar zit de waarde?”).

# Belangrijkste thema’s en onderwerpen
- Modelupdates en productgedrag: GPT‑5.1 (instant vs thinking) en wijzigingen in “persoonlijkheid”/sikofantie.
- Open source vs gesloten frontier-modellen: Moonshot AI’s Kimi K2 (1T parameters, MoE-activatie 32B) die op benchmarks dichtbij/over westerse topmodellen komt.
- AI-gegenereerde content en mediavertrouwen: schaalbaarheid van synthetische influencer-content, labeling/watermarks en het open-source lek.
- AI in consumer-producten: “tegen je foto’s praten” als nieuwe interface (Google Foto’s + “nano banana”).
- Enterprise-adoptie: McKinsey State of AI 2025—veel experiment, weinig brede uitrol en beperkte winstimpact, met kleine koplopersgroep.
- AI-industrienieuws/strategie: Yann LeCun (mogelijk) weg bij Meta richting world models; Microsoft/Satya Nadella’s visie dat de waarde in toepassingen/scaffolds zit, niet in modellen zelf.
- Nieuwe AI-tools/workflows: Sora 2 cameo-cloning + nieuwsfeed-automatisering; Gamma als AI-presentatie- en website-generator.

# Gebruiksscenario: AI-influencer flow met Sora 2 (Cameo) + nieuwsfeed + promptgeneratie
- Doel: automatisch “luchtige”, virale social video’s genereren die inspelen op actuele nieuwsitems.
- Componenten/programma’s:
  - **NOS feed** als inputbron voor actuele nieuwsitems.
  - **AI-model (ChatGPT/OpenAI-model)** als “prompt generator”: maakt formats/scriptjes die goed passen bij Sora.
  - **Sora 2** voor videogeneratie, inclusief **Cameo** (clonen van persoon op basis van kort filmpje + drie getallen uitspreken).
  - **(Beoogd) TikTok API** voor automatisch publiceren (nu nog niet volledig door te automatiseren).
- Workflow (zoals gebouwd/beschreven):
  1. Inlezen van nieuws via de **NOS feed**.
  2. Een AI-stap die eerst beoordeelt of een nieuwsitem “waardig” is om een video van te maken (kostencontrole, omdat genereren geld kost).
  3. Genereren van meerdere Sora-geschikte prompts/script-varianten per geselecteerd nieuwsitem.
  4. Handmatige stap: prompts in de Sora-app plakken, omdat de **Sora API** nog geen toegang biedt tot de **Cameo**-functie.
  5. Outputvideo’s publiceren (deels handmatig; doelbeeld is “zonder menselijke tussenstap” direct naar social).
- Observaties over prompting/kwaliteit:
  - Hoe **meer detail** in het prompt, hoe “stijver” of minder grappig het resultaat kan worden; **open prompts** leveren vaak creatievere/viraler aanvoelende video’s op.
  - Suggestie dat Sora “een TikTok-achtige” creatieve system prompt/temperatuur gebruikt: bedoeld voor standalone korte video’s, niet puur instructie-getrouw.
- Demonstratie-case:
  - Voor tv-programma **Eva** werd een item voorbereid met **Jort Kelder** als “ge-cameo’d” personage.
  - Zijn Instagram werd gevuld met AI-content; één video haalde ~**250.000 views**.
- Boodschap/impact:
  - “Als dit op een zolderkamer kan, kunnen anderen dit ook”: dit illustreert **informatie-inflatie** en de erosie van vertrouwen in wat je online ziet.

# AI-workflow: labeling/watermarks en het open-source probleem
- In Sora 2-video’s zit een vorm van **watermark/stenografie** waarmee platforms (bijv. TikTok) synthetische content kunnen herkennen en labelen als “generated”.
- Dit werkt vooral via **afspraken tussen modelproviders en platforms**.
- Probleem: bij **open modellen** (bijv. modellen van GitHub/Hugging Face-achtige distributie) kan watermarking:
  - ontbreken,
  - verwijderd worden,
  - of niet uniform afgedwongen worden.
- Conclusie: technische labeling is niet “oplossend” zolang open tooling watermarks kan strippen; er blijft een beleids-/handhavingsvraag: verantwoordelijkheid, verplicht labelen, omgang met open source.

# GPT‑5.1: wat er nieuw is en hoe het voelt in gebruik
- Release: OpenAI rolt GPT‑5.1 uit naar betalende gebruikers.
- “Twee smaken”: **Instant** en **Thinking** blijven, maar de **selectie** verandert:
  - Niet langer een externe “router” die bepaalt welk model wordt aangeroepen,
  - Maar het **model zelf** beslist wanneer het moet “nadenken” (trager, zwaarder) of snel antwoordt.
- Geclaimde verbeteringen:
  - **Beter instructies volgen** (instruction-following).
  - **Instant** zou “warmer/gezelliger” en speelser zijn; voorkeuren (zoals schrijfstijl) kunnen beter worden onthouden.
- Kritische observatie:
  - Risico op hernieuwde **sikofantie** (te veel meelullen/alles goed vinden), iets waar OpenAI eerder al op terug moest komen.
  - Onzekerheid of het een “echt nieuw model” is of vooral: system prompt + wrapper/scaffolding tweaks + bugfixes.
  - Geen uitgebreide benchmarks/PDF: voedt het idee dat dit vooral een **infrastructuur-/routingfix** is om kwaliteit én kosten te optimaliseren bij zeer grote gebruikersaantallen.

# Chinees open source model: Moonshot AI Kimi K2 (Thinking)
- Model: **Kimi K2 / Kimi K2 Thinking** van **Moonshot AI**.
- Positionering:
  - Scoort zeer hoog op benchmarks (o.a. **Humanity’s Last Exam** genoemd met **44,9%**).
  - Benadert/verslaat op delen westerse betaalde modellen.
- “Dubbel free”:
  - **Gratis te gebruiken** via Moonshot-hosting (webinterface),
  - én **vrij te downloaden**/zelf te hosten (open model).
- Gebruikservaring:
  - UI voelt als een **ChatGPT-kloon**; reasoning/“thinking traces” zijn uitgebreider zichtbaar (minder gecensureerd dan bij sommige Amerikaanse aanbieders).
- Praktische hardware-realiteit bij zelf hosten:
  - “Thuis draaien” is mogelijk maar zwaar: voorbeeld van ~**2× Mac Ultra** met veel geheugen (orde **€20.000**) om bruikbare tokens/sec te halen.
- MoE-architectuur (verklaring van “1T parameters maar 32B per vraag”):
  - Model is een **Mixture of Experts**: per prompt activeert het slechts een subset (“experts”) van het totale netwerk.
  - Voordeel: minder geheugen/compute per request dan een dicht 1T-parameter model.
- Trainingskosten als nieuwsfeit:
  - Moonshot claimt training rond **enkele miljoenen dollars** (bijv. ~4,1M genoemd), wat het “efficiëntiethema” (eerder DeepSeek-achtig) opnieuw aanwakkert.
- Implicatie: kloof tussen closed frontier en open modellen krimpt; al blijft het “inhaalspel” cyclisch wanneer closed labs nieuwe generaties uitbrengen.

# Gebruiksscenario: wanneer Kimi K2 wél/niet ChatGPT kan vervangen
- Potentieel “ja” voor:
  - Algemeen chatten, brainstormen, niet-gevoelige taken,
  - Experimenteren met reasoning traces,
  - Een extra model in een **ensemble** (meerdere modellen naast elkaar gebruiken).
- Potentieel “nee” of voorzichtig voor:
  - Gevoelige data (notulen, namen/adressen, interne documenten).
  - “Gratis” services impliceren vaak dat input mogelijk voor verbetering/fine-tuning gebruikt wordt; voorzichtigheid met privacy/compliance.
- Alternatief gedrag:
  - Voor “gesprekken die je niet in de trein zou voeren”: liever een meer vertrouwde/regionale oplossing (voorbeeld: **Le Chat/Mistral** werd genoemd als Europese optie), of een gesloten betaalde omgeving met beleid/contracten.

# Google Foto’s: “praten met Photoshop” via nano banana (niet in EU)
- Productnieuws:
  - **Google Foto’s** krijgt “nano banana” ingebouwd (beste beeldbewerkingsmodel volgens de podcast).
  - Je kunt foto’s aanpassen via natuurlijke taal: “verwijder zonnebril”, “open mijn ogen”, “laat mijn vriend lachen”, “zet me in een high fashion fotoshoot”.
- Gebruiksscenario:
  - Consumentenbewerking zonder toolkennis: geen lagen/maskers; enkel commando’s.
  - Snelle social-ready edits direct in je fotobibliotheek.
- Beschikbaarheid:
  - **Niet beschikbaar in Europa** (voorlopig), met verwachting dat dit later pas uitgerold wordt.

# McKinsey State of AI 2025: adoptie vs impact
- Kerncijfers:
  - **88%** van bedrijven gebruikt AI,
  - maar slechts **33%** heeft AI breed uitgerold,
  - en slechts **39%** ziet “een beetje” positieve winstimpact.
  - Een kleine kopgroep (**~6%**) schrijft **>5% winst** direct toe aan AI.
- Onderliggende boodschap:
  - Veel organisaties blijven steken in pilots/experimenten.
  - McKinsey identificeert best practices (31 werkwijzen getest), met nadruk op operationaliseren en schaal.
- Impliciete “root cause” (aansluitend op Dept-segment):
  - AI-transformatie is vaak een **dataformatie**: datakwaliteit, beschikbaarheid, infrastructuur, talent en werkwijzen bepalen of AI echt rendement oplevert.

# Dept (sponsor): AI-transformatie als data- en organisatievraagstuk
- Stelling:
  - Voor veel merken ligt de bottleneck niet bij “welk model”, maar bij **datafundament**, **manier van werken**, **talent** en **technische infrastructuur**.
- Aanpak/gebruiksscenario:
  - Begin met een **heldere visie**: wat moet AI de komende jaren opleveren?
  - Breng vervolgens randvoorwaarden en capabilities in kaart.
  - Vermijd losse **point solutions** die niet schaalbaar zijn in impact.
- Context:
  - Dept noemt ervaring bij o.a. Lufthansa en een retailmerk (genoemd), en positioneert dit als route van experiment naar organisatiebrede implementatie.

# AI-industrienieuws: Yann LeCun en Meta, focus op world models
- Nieuws:
  - **Yann LeCun** zou Meta verlaten om een startup te starten; in gesprek met investeerders.
- Focus van de startup:
  - **World models**: systemen die leren via interactie/causaliteit in de echte wereld, niet alleen door eindeloos data te “consumeren”.
- Meta-context:
  - Meta zou AI-strategie omgegooid hebben: nieuwe divisie, Alexander Wang binnengehaald, veel hires met hoge bedragen.
  - Signalen van interne chaos; vertrek zou daarmee verklaarbaar zijn.

# Microsoft/Satya Nadella bij Dwarkesh: “waarde zit in scaffolding, niet in modellen”
- Observatie uit interview:
  - Rondleiding door Microsoft-datacenter; schaalflex: één datacenter met capaciteit “10× GPT‑5 training” (zoals aangehaald).
- Strategisch standpunt:
  - Modellen zelf zijn minder verdedigbaar (worden gekopieerd/open source), terwijl de **applicatie-laag** (Excel, Windows, ecosystemen) de echte slotgracht vormt.
- Gebruiksscenario: “Excel agent” / middle tier AI
  - AI krijgt context + tools/toegang binnen Excel:
    - begrijpt je sheet,
    - kan handelingen uitvoeren,
    - combineert foundation model + Excel-specifieke handleiding + tool-toegang.
  - Doel: gebruikers “praten met Excel” in plaats van zelf spreadsheets bouwen.
- Implicatie:
  - Als agents steeds beter worden, verschuift de interface: minder “spreadsheets maken”, meer “doel formuleren en antwoorden krijgen”, eventueel met onder-de-motorkap controle.

# Nieuwe tool: Gamma (AI-presentaties) + workflow naar website
- Toolnieuws:
  - **Gamma**: AI-presentatietool, winstgevend, ~52 medewerkers, waardering ~**$2,1B**.
- Gebruiksscenario’s en functies:
  - **Prompt → presentatie**: genereert complete decks met conceptslides, layouts, kleuren en fonts op basis van instructies.
  - Voorbeeldprompt: campagne voor minimalistische sneakers, doelgroep Gen Z, doel 10.000 pre-orders, focus influencers + paid social.
  - **Convert to website**: één klik om een deck om te zetten naar een **live website** (publiek te delen).
  - Extra’s:
    - Diagrammen en flowcharts genereren (gedachten → schema),
    - **Presentation analytics**: inschatting waar publiek afhaakt.
- Praktische inzet (zoals besproken):
  - Vooral nuttig als **ideation/prototyping**: meerdere decks laten maken, beste slides/visualisaties hergebruiken in eigen presentatie.
  - Ook als uitlegvorm: een boek/complex onderwerp laten uitleggen “in slides” om sneller te scannen dan een tekstsamenvatting.

# Overige opvallende punten
- GPT‑5 routingcontroverse:
  - Eerder probleem: gebruikers kregen te vaak een lichter model (GPT‑5 mini-achtig) door routering; 5.1 probeert dat te verbeteren door de beslissing in-model te leggen.
- Chip- en infra-discussie:
  - Vermindering van afhankelijkheid van Nvidia: alternatieve chips voor training/inference (o.a. Amazon’s chips voor Anthropic-infra genoemd) en gespecialiseerde inference-hardware.
- Europa-achterstand in features:
  - Google Foto’s AI-editing (nano banana) voorlopig niet in EU—illustratie van regionale beperkingen/regulatoire frictie.