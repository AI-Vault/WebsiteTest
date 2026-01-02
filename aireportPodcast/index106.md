# 106. Google lanceert AI de ruimte in + Apple Intelligence nu in Nederland + robot krijgt existentiële ... (2025-11-07) [link](undefined)


 De snelle verschuiving van AI van “handige software” naar zware infrastructuur en geïntegreerde productfeatures: van energie/compute (zelfs in de ruimte) tot AI-assistenten in consumentenproducten (Google Maps, Siri) en praktische AI-workflows voor commerce, robots en visualisatie.

# Belangrijke thema’s en onderwerpen

# AI-debat en maatschappelijke frictie: “AI maakt ons dom”
- Er wordt vooruitgeblikt op een publiek debat (met o.a. Erik Scherder en Matthijs van Nieuwkerk) rondom het idee dat AI negatieve effecten heeft op cognitieve vermogens, leren en actieve hersengebruik.
- Voorbeeld uit het onderwijs: studenten die betrapt worden op ChatGPT-gebruik bij papers; vervolgens gebruiken ze ChatGPT óók voor het schrijven van excuusmails (met herkenbare stijlkenmerken zoals “mdashes”), wat de discussie voedt over afhankelijkheid en gemakzucht.

# AI-infrastructuur en energie: datacenters in de ruimte (Google “Project Suncatcher”)
- Google werkt aan “Suncatcher”: satellieten met zonnepanelen en AI-chips die AI-modellen in een baan om de aarde moeten trainen.
- Rationale:
  - In de ruimte leveren zonnepanelen tot ~8× meer energie dan op aarde (geen atmosfeer/bewolking).
  - Energie is een nieuwe bottleneck: Microsoft’s CEO noemt AI-chips die ongebruikt blijven door energietekort (niet door chip-tekort).
- Opzet en techniek:
  - Eerste stap: twee prototypes in 2027.
  - Opereren op zeer lage baan (~650 km) en zeer dicht bij elkaar (honderden meters tot enkele kilometers) om voldoende bandbreedte/latency te halen.
  - Doel: een “swarm/constellation” die onderling via optische (laser)communicatie data uitwisselt, analoog aan GPU’s in een datacenter die zich als één “meta-computer” gedragen.
- Economische haalbaarheid:
  - In de bijbehorende research paper wordt doorgerekend wanneer het rendabel kan worden, vooral door dalende lanceerkosten (prijs per kg naar orbit) en groeiende beperkingen op aarde (regelgeving, energietekorten, geopolitiek).
  - Verwachte omslagpunt: ergens tussen 2030–2040 (mid-2030s als indicatie).
- Extra nuance:
  - Het gaat om training, niet inference (dus niet “jouw prompt via satelliet”).
  - Afvoer van warmte is in de ruimte “makkelijker” (warmte wegstralen), in contrast met lokale opwarming/koelingsproblemen op aarde.

# AI-infrastructuurtrend: “GPU in de ruimte” (Starcloud)
- Start-up Starcloud lanceert test-satelliet “Starcloud 1” (formaat kleine koelkast, ~60 kg) met een Nvidia H100 GPU.
- Nog geen grote constellation, maar illustreert dat “compute in space” breder leeft dan Google.

# Productintegratie: Google Maps krijgt Gemini-integratie (conversational navigation)
- Google Maps wordt “gespreksgestuurd” door Gemini:
  - Natuurlijke taalvragen zoals: “een betaalbaar vegan restaurant langs mijn route”.
  - Gemini doorzoekt ~250 miljoen bedrijven, weegt reviews en foto’s mee en geeft gepersonaliseerde suggesties.
- Nieuwe use-cases in combinatie met apps/services:
  - Tijdens navigatie agenda-items toevoegen (“zet voetbaltraining morgen 17:00 in mijn agenda”) – cross-app integratie met Google Calendar.
  - Gevaren melden via spraak (handsfree) i.p.v. tikken/keuzemenu’s: bijvoorbeeld een stilstaande auto met knipperlichten, obstakel of “dood dier” op de weg.
  - Context-specifieke instructies: navigeren op herkenningspunten (“rechtsaf bij het tankstation/rode café”), mogelijk gemaakt door koppeling met Street View-beelden en Maps-database.
  - Proactieve waarschuwingen op frequente routes (woon-werk): meldingen over ongevallen, wegwerkzaamheden, afsluitingen vóór vertrek.
  - Google Lens binnen Maps: camera op gebouw/monument → Gemini geeft direct uitleg/achtergrond.
- Uitrol: “komende weken” naar Android én iOS.
- Thema eronder: integratie van foundation models in bestaande producten kost tijd door legacy-infrastructuur en “silo’s” in grote organisaties; Microsoft rolt snel uit (Copilot), maar kwaliteit/afwerking varieert.

# Apple en AI-strategie: Siri “slim maken” via Google Gemini (gelekt)
- Volgens Bloomberg betaalt Apple ~$1 miljard per jaar aan Google om Siri te verbeteren via een aangepast Gemini-model.
- Belangrijk detail: dit model draait op Apple’s eigen servers (on-prem/cloud onder Apple-beheer), niet als simpele “doorstuur-API”.
- Modelgrootte: genoemd wordt ~1,2 biljoen parameters, veel groter dan Apple’s huidige cloudmodel (~150 miljard).
- Positionering in Apple’s stack:
  - Siri (oude laag) + Apple Intelligence (nieuwe laag, lokaal + cloud) + optioneel ChatGPT als “fallback/plug-in”.
  - De gelekte Gemini-deal lijkt een volgende stap: Apple Intelligence-cloud die krachtiger wordt door gelicenseerde, aangepast getunede Gemini-capaciteit.
- Verwachte impact voor gebruikers:
  - Meer belofte-inlossing van Apple’s “personal context”-visie: systeem-brede assistentie die data uit apps/berichten/agenda begrijpt en acties uitvoert (planning, samenvatting, contextuele taken).
- Strategische duiding:
  - Apple “build vs buy”: tijdelijk inkopen om de achterstand te dichten, terwijl Apple intern verder bouwt of mogelijk inzet op (kleine of grote) acquisities/strategische investeringen.
  - Anthropic wordt genoemd als populaire enterprise-keuze (en al sterk in programmeren), maar in de Apple-onderhandeling zou Anthropic “te duur” zijn geweest.

# AI-gerelateerd nieuws: Apple Intelligence in Nederland beschikbaar
- iOS-update brengt Apple Intelligence naar het Nederlands (voor recente iPhones met voldoende rekenkracht).
- Concrete use-cases:
  - Tekstcorrectie/rewrite/samenvatten direct in het toetsenbord/system-wide selectie-menu.
  - Verbeterde dicteerfunctie (spraak-naar-tekst) door modernere taalmodellen.
  - Optioneel: taken kunnen naar ChatGPT worden doorgestuurd (met/zonder account), maar basisfuncties draaien primair in Apple’s eigen omgeving.

# AI-bedrijfsnieuws: Anthropic financiële groei
- Anthropic mikt op ~$30 miljard omzet in 2028; verwacht ~$3,8 miljard inkomsten dit jaar.
- Verwachte winstgevendheid in 2028, terwijl OpenAI naar verwachting langer verlieslatend blijft (tot ~2029).
- Groei komt vooral uit enterprise-deals (o.a. Microsoft, Salesforce, Deloitte).
- Positionering: Anthropic als favoriet bij grote bedrijven; vooral programmeercapaciteiten van Claude-modellen zijn gewild.

# Robots + generieke LLM’s: “ButterBench” (stofzuigerrobot die boter moet brengen)
- Onderzoek test hoe generieke modellen (GPT, Claude, Gemini) robot-taken kunnen aansturen zonder specifieke robottraining.
- Setup:
  - Een Roomba-achtige robot met camera’s en een 3D-geprint “plateau” op de rug.
  - Opdracht: boter herkennen tussen objecten, vinden, vervoeren naar een mens die zich verplaatst naar een andere kamer.
- Twee lagen in prestaties:
  - Orchestratie/planning en situational awareness (via beelden interpreteren, plan maken) gaat relatief goed.
  - Fine-grained motor control (precies draaien, bewegen, interactie met omgeving) gaat zwak; modellen raken “stuck” in herhaald corrigeren (“15 graden draaien”, foto nemen, terugdraaien, etc.).
- Opvallend fenomeen: “emotionele” interne monologen
  - In logs lijken modellen stress/paniek te simuleren bij lege accu of falende docking (“catastrophic cascade error”, quasi-existentiële zinnen).
  - Interpretatie in de bespreking: dit is vooral stijl/tekstproductie op basis van trainingsdata (sciencefiction/psychologie), maar het roept wél empathische reacties op en voedt publiek debat over “bewustzijn”.

# Gebruiksscenario’s: direct verkopen via ChatGPT (Dept) + gebruikte programma’s
- Context: OpenAI kondigt aan dat direct shoppen/afrekenen binnen ChatGPT mogelijk wordt; eerste integraties met Etsy (VS live) en Shopify.
- Probleem voor merken:
  - Wat als je e-commerce niet op Shopify draait, maar je wel direct in ChatGPT wilt kunnen verkopen?
- Dept’s oplossing / workflow:
  - Een “Shopify engine” naast de bestaande webshop: een Shopify-omgeving die parallel draait (“naast je shop zetten”).
  - Doel: zonder volledige migratie of ombouw tóch kunnen aansluiten op ChatGPT’s commerce-flow zodra beschikbaar.
- Vereisten voor verkoop via ChatGPT:
  - Productvindbaarheid: je PIM/productdatabase zó ontsluiten dat ChatGPT producten kan vinden en ophalen.
  - Frictieloos afrekenen: bestellen en betalen binnen ChatGPT (zodra de functionaliteit live is).
- Programma’s/platformen die expliciet langskomen:
  - ChatGPT (als shopping interface)
  - Shopify (als transactielaag/commerce platform)
  - Etsy (eerste live partner)
  - PIM/product database (als bron voor productdata)

# Nieuwe tool: Napkin AI (tekst → infographics/flowcharts/diagrammen)
- Functionaliteit:
  - Zet tekst om in professionele visuals zoals infographics, flowcharts en diagrammen, zonder designervaring en zonder handmatig layouten.
- Praktijkscenario (redactie):
  - Input: losse iPhone-notities met film-pitch (dialogen, character arcs, cinematografie-ideeën) – “complete chaos”.
  - Workflow: notities uploaden naar Napkin AI → output binnen minuten: flowcharts en storyboard-achtige structuur → resulteert in een coherent verhaal/pitch.
- Extra features:
  - Style library: huisstijl instellen (kleuren, fonts, merklook) zodat outputs consistent in meerdere stijlvarianten kunnen worden gegenereerd.
- Positionering:
  - Specifieke tool die beter past voor “visualiseren van tekst” dan generieke chatbots die óók plaatjes kunnen maken, maar minder doelgericht zijn voor diagrammen.

# Overkoepelende observaties
- AI-ontwikkeling splitst in twee sporen:
  - Infrastructuur/energie: extreme oplossingen (ruimte-constellations) door groeiende compute- en energievraag.
  - Productisatie: per app/product concrete verbeteringen (Maps, Apple Intelligence), waarbij integratie traag kan zijn door legacy en organisatie-silo’s.
- Tegelijk neemt enterprise-adoptie toe (Anthropic), terwijl consumenten-UX verschuift naar “AI zit er gewoon in” (Maps) en commerce in conversational interfaces (ChatGPT shopping).