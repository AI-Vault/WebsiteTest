# 115. Claude ruimt je rommel op + Siri wordt slim met hulp van Google + OpenAI en Anthropic lanceren AI... (2026-01-15) [link](undefined)


 # De snelle verschuiving van “AI als chat” naar “AI als agent” die daadwerkelijk werk uitvoert in je digitale omgeving (bestanden, aankopen, persoonlijke data en gezondheidsdossiers), met nieuwe producten van Anthropic/Claude, OpenAI/ChatGPT, Google/Gemini en Apple.

# Cloud Cowork (Anthropic/Claude): werken in jouw mappen met parallelle agents
- **Wat het is**: een nieuwe modus in de Claude desktop-app (“Cowork”) waarmee Claude toegang krijgt tot één geselecteerde map op je Mac en daar bestanden kan **lezen, bewerken, aanmaken, hernoemen en structureren** (documenten, spreadsheets, presentaties).
- **Belangrijkste vernieuwing**: grote opdrachten worden door Claude eerst opgeknipt in **subtaken** die **parallel** draaien. Je ziet voortgang en tussenstappen; Claude stelt ook **verduidelijkende vragen** voordat het ingrijpende acties uitvoert.
- **Beschikbaarheid & prijs**: op dit moment **alleen Mac**, en alleen voor het **Claude Max-abonnement (~€90/maand)**.

# Gebruiksscenario’s met Cloud Cowork (concrete voorbeelden)
- **Financiën / abonnementen opschonen (CSV-banktransacties)**  
  - Gebruiker dumpt **banktransacties (CSV)** in een map en vraagt om een overzicht van abonnementen én om ze direct op te zeggen.  
  - Cowork kan vervolgens een **browser openen** en opzegprocessen doorlopen.  
  - Het lukt niet altijd, maar bij sommige (bijv. Stripe-achtige flows) gaat het wél vlot.  
  - Resultaat: “blik in de toekomst” waarin AI niet alleen analyseert, maar ook uitvoert.
- **Downloads-map opruimen en structureren**  
  - Prompt: “Orden mijn Downloads-map op thema.”  
  - Cowork maakt submappen (bijv. “Facturen”) en verplaatst bestanden automatisch.
- **Bonnetjes/facturen → spreadsheet → presentatie**  
  - Cowork kan bedragen uit bonnetjes halen, een **spreadsheet** maken en zelfs een **PowerPoint** genereren met een gewenste stijl/structuur.
- **Daytrader belastingmatching**  
  - Een taak die eerder $700/jaar kostte (trades matchen voor belastingaangifte) wordt “één prompt”.
- **Designer workflow**  
  - “Organiseerde mijn rommelige bureaublad terwijl ik naar de wc ging.”
- **Ondernemer: 2 maanden achterstallig werk in 2 uur**  
  - Cowork produceert o.a. **vacatureteksten**, marketingstrategie met budgetallocatie, bulk e-mails, website-copy, LinkedIn-reacties.
- **Podcast-host: thematische analyse op grote schaal**  
  - Cowork krijgt toegang tot **320 transcripties** en levert in ~15 minuten de **10 belangrijkste thema’s** (werk dat normaal dagen kost).
- **Schrijver/redacteur: drafts vs. gepubliceerd werk**  
  - Cowork vergelijkt lokale concepten met gepubliceerde artikelen en maakt een overzicht van welke drafts nog waardevol zijn.

# Nieuwe workflow/architectuur: “Claude Code → Cowork” (zelfde motor, nieuw “harnas”)
- Cowork wordt gepositioneerd als een **gebruiksvriendelijker ‘schilletje’** bovenop technieken die programmeurs al kennen uit **Claude Code** (agentic, tool-using, langlopende taken).
- Kerninzicht: de “Superman-pakken/harnassen” die voor programmeurs zijn gebouwd, worden nu vertaald naar **kantoortaken**: mappen opschonen, documenten maken, rapportage, etc.
- Opvallend detail: Cowork is **met Claude Code gebouwd** in **~anderhalve week** (onder supervisie), met de claim dat er **geen traditionele ‘regelcode’** geschreven hoefde te worden. Dat wordt neergezet als indicator van volwassenwording van AI-assisted development.

# Risico’s en aandachtspunten bij Cowork/agentic tools (privacy & veiligheid)
- **Nondeterminisme**: je kunt niet exact voorspellen wat het systeem doet; herhaalde runs kunnen anders uitpakken.
- **Te “behulpzaam” gedrag**: agents kunnen creatief worden in het behalen van doelen en verder gaan dan de gebruiker bedoelde.
- **Praktisch risico**: per ongeluk hernoemen/verplaatsen/verwijderen van bestanden (dus: werken met testmappen/back-ups).
- **Groter risico**: data kan (bedoeld) via web/tools bij derden belanden, bv. als Claude “een externe tool” zoekt om transacties te categoriseren.
- Discussiepunt (Simon Willison): voor gewone gebruikers is “let op verdachte acties” moeilijk te beoordelen; daarom niet gebruiken voor gevoelige data (financieel/medisch) zolang guardrails niet robuust genoeg zijn.
- Fenomeen “YOLO-modus” (expliciet of impliciet): continu op “ja” klikken zonder te begrijpen is functioneel hetzelfde als alle toestemming geven.

# Persoonlijke productiviteit: Obsidian + Claude Code als “besturingssysteem-assistent”
- **Obsidian** wordt uitgelegd als notitie-app waar alles lokaal staat als **Markdown-bestanden** in mappen op je schijf (i.t.t. Notion/Apple Notes met databases).
- Workflow: exporteer taken uit een to-do app (bijv. **Superlist** via GDPR-export/CSV), geef Claude Code toegang tot de Obsidian-map + CSV + screenshots, en laat het:
  - een passende **Obsidian-plugin** kiezen/instellen om to-do functionaliteit te repliceren,
  - taken importeren inclusief tags/projecten,
  - discrepanties corrigeren op basis van screenshots.
- Resultaat: de gebruiker ervaart een nieuwe werkwijze waarin Claude “naast” de todo-UI staat en ook toegang heeft tot notities/vergadercontext, waardoor je **in natuurlijke taal je dag plant**, taken herschikt, conceptmails laat opstellen, enz.
- Breder thema: “als data lokaal en open is, kan AI er veel makkelijker mee werken”—een herwaardering van lokale bestanden/open standaarden.

# Apple maakt Siri “slim” via Google Gemini (maar met Apple-controle)
- Apple kondigt aan dat **Gemini** de motor wordt achter de vernieuwde Siri:
  - Siri gaat van “zoekresultaten” naar **echte antwoorden** zoals bij ChatGPT/Gemini.
  - **Apple houdt controle**: AI draait op **Apple’s eigen servers**, Google krijgt **geen toegang tot gegevens**.
  - **Geen Gemini-branding** zichtbaar; het wordt verweven in iPhone/Siri.
  - Eerste functies: **dit voorjaar**.
- Thema: grote platformbedrijven willen wel topmodellen, maar zonder datamodel/branding uit handen te geven.

# AI-commerce: Google’s Universal Commerce Protocol + conversational checkout
- Google lanceert **gepersonaliseerd shoppen met AI**: gesprek i.p.v. lijst met links.
- **Universal Commerce Protocol (UCP)**:
  - Een **standaard/protocol** waarmee AI-assistenten producten kunnen zoeken/vergelijken en vervolgens **afrekenen** (o.a. via **Google Pay**) zonder de chat te verlaten.
  - Vereist deelname van winkels én integratie via payment providers; werkt dus met een soort **allow-list** van partners.
- Context: dit past in een bredere trend:
  - ChatGPT lanceerde eerder een checkout-functie,
  - Microsoft volgde met Copilot checkout.
- Strategisch debat:
  - AI wordt de nieuwe “air traffic controller” voor retail (de interface waar beslissingen vallen).
  - Marktplaatsen/retailers (bol.com/Coolblue) riskeren te worden overgeslagen, tenzij ze waarde toevoegen (logistiek/retourdata/advies/ervaring/branding).
  - Tegengeluid: net als “online vs. offline” verdwijnt niet alles; sommige koopervaringen blijven waardevol via merkwebsites en fysieke winkels.

# AI in de zorg: “AI doctor” bij OpenAI en Anthropic
- Beide bedrijven introduceren extra medische functionaliteit:
  - Je kunt **medische dossiers uploaden** (labuitslagen, consultsamenvattingen, klinische geschiedenis) en vragen stellen als:
    - “Hoe ontwikkelt mijn cholesterol zich?”
    - “Kun je mijn bloedonderzoek samenvatten voor mijn afspraak?”
- Grote vraag vanuit gebruikers:
  - 230 miljoen mensen stellen wekelijks gezondheidsvragen aan ChatGPT; ~**1 op de 5** gebruikers doet dit.
- Belangrijke productdetails (vooral bij OpenAI genoemd):
  - **Apart health-tabblad/modus**.
  - **Gescheiden memory/silo** voor medische context (niet vermengd met algemene chats).
  - Extra “scaffolding”: langer nadenken, checks tegen hallucinaties, claims dubbel/triple-checken (duurder, maar bedoeld voor hogere betrouwbaarheid).
  - Koppelingen met **Apple Health** en **MyFitnessPal** (genoemd bij ChatGPT Health).
- Discussiethema’s:
  - **Kwaliteit/veiligheid**: risico op hallucinaties en bevestigingsbias (bijv. bij hypochondrie).
  - **Privacy & toezicht**: geen artsenplicht/medisch beroepsgeheim zoals bij artsen; onduidelijk toezicht.
  - **Maatschappelijke druk**: van vrijwillige quantified-self naar mogelijke norm/verwachting (“moeten we dit willen?”), preventie vs. neurose/overmonitoring.
  - Data-honger: verwijzing naar Elon Musk die publiek oproept medische data te uploaden naar Grok om het model te verbeteren (AI-trainingsprikkel als drijfveer).

# Google Personal Intelligence: Gemini met jouw persoonlijke data (VS)
- Google kondigt aan dat Gemini persoonlijke antwoorden kan verbeteren door combinaties van:
  - **Gmail**, **Google Foto’s**, **zoekgeschiedenis**, **YouTube-kijkgedrag**.
- Voorlopig alleen in de **VS**.
- Implicatie: AI-assistenten bewegen richting “gegrond in jouw leven” (context), vergelijkbaar met Cowork’s toegang tot je computer, maar dan op cloudplatformniveau.

# Marketing/onderzoek: synthetische AI-persona’s (Dept)
- Tooling/aanpak:
  - Train een AI op **historische klantdata** (onderzoeken, gebruikersdata).
  - Marketeers kunnen **in gesprek** met het model alsof ze realtime met doelgroepen praten.
  - Validatie is nodig om te voorkomen dat de persona’s “onzin” geven.
- Gebruiksscenario’s:
  - Sneller testen van **productconcepten**, **customer journeys** en **campagnes** zonder traditionele focusgroepen.
  - In uren inzicht in prijslogica, boodschap-fit, frictiepunten in journey; continu beschikbaar en schaalbaar.

# Tool-tip: Huxe (van ex-NotebookLM-makers) – persoonlijke interactieve ochtendpodcast
- App: **HUXE** (H U X E).
- Workflow:
  - Koppelt aan je **Google-account** (e-mail, agenda, adressen).
  - Genereert een **persoonlijke ochtendbriefing** (~5 minuten) met nieuws dat voor jou relevant is + dagoverzicht.
  - Interactief: je kunt hosts **onderbreken** en vervolgvragen stellen (zoals bij NotebookLM audio).
- Gebruiksscenario:
  - Tijdens pendelen/multitasken: snel overzicht van je dag en context bij nieuws; je kunt direct verduidelijking vragen.
- Kanttekeningen:
  - Vereist toegang tot e-mail/agenda (privacy-implicaties).
  - Gratis versie is beperkt.
  - Beschikbaar via **Apple App Store** en **Google Play Store**.

# AI-gerelateerd nieuws (samengevat)
- Anthropic: **Claude Cowork** (agentic bestandswerk op Mac; parallelle taken; Max-abonnement).
- Apple: **Siri** wordt slimmer met **Google Gemini**, draaiend op Apple-servers zonder Google data-toegang/branding.
- Google: AI shopping + **Universal Commerce Protocol** + checkout via **Google Pay**; richting webshops “in de chat”.
- OpenAI & Anthropic: medische functies (“AI doctor”/health-modus) met upload van dossiers en health-vragen.
- Google: **Personal Intelligence** (Gemini met Gmail/Photos/Search/YouTube) in de VS.
- Dept: synthetische AI-persona’s voor sneller marketing-/innovatieonderzoek.
- Huxe: interactieve gepersonaliseerde morning briefing/podcast op basis van Google-data.