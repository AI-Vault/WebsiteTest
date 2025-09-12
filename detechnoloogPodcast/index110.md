# 110. Wanneer breekt het eerste AI-device écht door? (2025-07-24) [link](https://www.youtube.com/watch?v=RjFWcvdfYQ0)


 # Hoofdonderwerp
Realtime, mensgerichte AI — hoe ontwerp je apparaten en algoritmes die in real time met mensen meeleven, leren en veilig handelen (met aandacht voor vormfactor, privacy en praktische adoptie).

# Belangrijkste thema's
- Vormfactor: welk device (bril, pin, oorstukje, smartphone, horloge) levert daadwerkelijk meerwaarde?  
- Realtime leren en adaptatie: AI die niet alleen uitgerolde modellen gebruikt, maar in-the-moment leert en onzekerheid kwantificeert.  
- Mensgerichte interactie: systemen ontwerpen vanuit menselijke routines, aandacht en fouten (action vs. learning).  
- Wiskundige/architectuurverandering: neuromorfische modellen, Bayesiaanse/normalverdelingbenadering en Active/Interactive Inference.  
- Privacy, energie en productie: edge computing, data minimalisatie, EU-regulering en manufacturability/design.  
- Huidige experimenten vs. massamarkt: voorbeelden van vroege devices, wat werkt, wat niet.

# Gedetailleerde weergave
Het gesprek (Roel en andere deelnemers) verkent decennia aan experimenten met draagbare AI-apparaten (van vroeg-2000s prototypes tot de Humane AI Pin en Rabbit R1) en verbindt die praktijk met actuele AI-architectuurvragen. Kernidee: huidige generatieve AI (LLM's, multimodale modellen) is krachtig voor veel routines, maar mist twee cruciale eigenschappen van menselijke intelligentie:
- realtime online leren (gebruikmaken van één of enkele observaties om hypotheses aan te passen), en  
- expliciete onzekerheidskwantificatie (inschatten hoe zeker je bent en hoe groot de variantie is).

Roel betoogt dat je wiskunde en rekenmodellen moet veranderen: in plaats van enkel punt-schattingen te gebruiken, werk met distributies (normaalverdelingen), Bayesiaanse updates per observatie (hij noemt een "Piaanse vergelijking") en een Active/Interactive Inference-benadering (gebaseerd op Carl Friston) om continu voorspellingen te maken, afwijkingen te meten en vervolgens te leren of te handelen. Dit reduceert wat geleerd moet worden: alleen het verschil tussen voorspelling en werkelijkheid hoeft te worden verwerkt.

Er worden concrete experiments en voorbeelden besproken:
- Eye-tracking & aandacht: systemen die meten of iemand kijkt, gebruiken dat om voorkeuren/interruptibility te bepalen. Roel refereert aan werk uit eind jaren '90 en vroege 2000s dat al eye-tracking-toepassingen bouwde.  
- Autorijden (simulator experiment): een “bumperkleef”-experiment toonde dat mentale belasting kwadratisch stijgt met een maat die gerelateerd is aan afstand/snelheid (variabiliteit). Een AI kan op basis van afstand/variabiliteit inschatten hoeveel cognitieve ruimte een bestuurder nog heeft en interface (navigatie zoom in/uit), meldingen of gesprekken adaptief regelen. Dit kan zonder traag tastbare fysiologie-sensoren (HRV/EMG), puur via afstand en visuele data (camera/LiDAR/radar).  
- Advertentie-analytics (Zuk): privacyvriendelijke gaze-telling (tel alleen oogballen en gooi videodata weg) om publiciteitsprestaties te meten zonder identiteitsdata te bewaren.  
- Humane AI Pin & Rabbit R1: vroege commerciële pogingen — veelbelovend qua vormexperimenteel, maar beperkte meerwaarde t.o.v. smartphone; kosten en abonnementen beperkt adoption.  
- ChatGPT & camera: huidige apps kunnen camera-input gebruiken en objecten beschrijven, maar dit is grotendeels supervised en afhankelijk van gelabelde datasets; weinig echte on-device, snelle personalisatie.  
- Voice bots (DHL ervaring): spraakinterfaces blijven inconsistent; gebruikerservaring kan frustrerend zijn en soms leidt directe spraakherkenning tot snel schakelen naar menselijk contact.

# Gebruikscases en gebruikte programma's / systemen (gedetailleerd)
- Autorij-assistent (gebruikte technieken en programma's):
  - Input: camera/LiDAR/radar op voertuig; verkeerscontext (snelheid, afstand).  
  - Model: realtime Bayesiaanse/Active Inference module die per frame/update de verwachting en onzekerheid bijwerkt.  
  - Output: adaptieve HMI (navigatie in-/uitzoomen), waarschuwingen, automatisch remmen of aanbevelen tot actie.  
  - Programma/stack voorbeelden: simulators voor experimenten; op device inferentie- en update-modules (edge runtime, eventueel neuromorphic hardware).  

- Persoonlijke assistent / companion:
  - Input: audio (spraak), eventueel camera (context), kalender/drive/agenda (optionele data).  
  - Model: realtime adaptieve model dat routines (basale ganglia) en persoonlijke voorkeuren combineert — leert snel on-device met weinig data.  
  - Use cases: manager-assistent (agendamanagement, e-mailvoorstellen), contextgevoelige suggesties (niet storen tijdens podcast), en “butler”-achtige services.  
  - Programma/stack: LLM/ multimodaal backend + on-device interactive inference laag; integraties met Google Drive/Gmail/kalenders (met privacy design).  

- Vision/beeld + Chat (ChatGPT app met camera / multimodale modellen):
  - Use: objectherkenning, scene description, snelle Q&A over beelden.  
  - Programma: ChatGPT multimodal features of Google multimodal / Gemini. Werkt vaak via cloud en gelabelde datasets (supervised), soms met menselijke labelers als ondersteuning.

- Advertentie-analytics (Zuk):
  - Input: camera-feed bij scherm, privacy-first pipeline (tell-only gaze, drop raw video).  
  - Output: metriek voor ad exposure; real-time aanpassing van content.  
  - Programma: eenvoudige computer vision gaze-detectie en analytics-dashboard.

- Voice bots / klantenservice (DHL):
  - Input: telefonische spraak, intent-classifier.  
  - Output: dialoogsturing, escaleren naar mens als frustratie/hectiek.  
  - Programma: spraak-naar-tekst, intent recognition, fallback-to-human.

# Nieuwe tools en AI-workflows vermeld
- Interactive Inference: afgeleide van Carl Friston’s Active Inference; vereenvoudigde versie toegepast op mens-computerinteractie. Workflow: model voorspelt zintuiglijke input → vergelijk met werkelijke input → bij afwijking beslis je (actie) of update model (leren). Sleutel is per-observatie Bayesiaanse updates, leren alleen van fouten (prediction errors) — efficienter dan brute-force offline training.
- Edge realtime learning workflow: per-observatie Bayesiaanse updates (normaalverdelingsrepresentatie), kwantificatie van onzekerheid (niet alleen top-score), en on-device inferentie/training om latentie en privacy te verbeteren.
- Neuromorfische informatica: genoemd als pad naar extreem efficiënte, laag-energie realtime leren die het menselijke brein benadert qua energiegebruik (voorbeeld: menselijke hersenen werken op wattages die extreem laag zijn vergeleken met datacenters).
- Agents & large-action models: refereert aan apparaten die acties over API’s willen uitvoeren (bv. bestellen via Uber) maar geconfronteerd worden met integratie-problemen (API-ecosysteem, inconsistentie).
- Bayesiaanse / “Piaanse vergelijking” updates: per-observatie kans- en onzekerheidsupdate (transcript gebruikt term “Piaanse vergelijking” voor de wiskundige update — idee: reken per observatie de kans tov je eerdere kennis).

# AI-nieuws genoemd in het gesprek
- Gemini presteerde sterk op een wiskundeslag/competitie (genoemd als “wiskunde olympiade” — resultaat: goed maar niet perfect).  
- Sam Altman / aankoop van Johnny Ive’s designbedrijf door Sam Altman (er wordt verwezen naar dat zakelijke nieuws en de mogelijke impact).  
- Google/andere bedrijven ontwikkelen multimodale modellen en smart glasses prototypes (Snap Spectacles demo, Google demonstraties).  
- Kritiek op Apple’s Vision Pro positionering; discussie of Apple de boot heeft gemist op AI-device integratie en of Apple “Apple Intelligence” slechts PR is.

# Praktische uitdagingen en aandachtspunten
- Vormfactor & adoptie: gebruikers willen geen extra klunky apparaat; device moet modieus, licht en duidelijk meerwaarde hebben ten opzichte van smartphone, horloge, AirPods of bril.  
- Privacy en wetgeving: EU AI Act en publieke gevoeligheid bij camera’s vereisen privacy-by-design (bv. tel-alleen-gaze en drop raw video).  
- Energie & compute: realtime on-device leren vergt efficiënte hardware (neuromorphic, spaarzame representaties) om niet steeds naar cloud te moeten.  
- Data & context: echte world observations (niet alleen webdata) zijn nodig voor contextuele beslissingen; training op video (YouTube e.d.) helpt, maar on-device persoonlijk leren is cruciaal voor gepersonaliseerde assistenten.  
- Integratie & API-ecosysteem: agents en action-models falen vaak door gebrek aan gestandaardiseerde, betrouwbare integraties (bestelling/tracken etc.).  
- User experience: aandacht, interruptibility en etiquette (bv. moet AI weten wanneer niet te luisteren, of wanneer in te grijpen) vragen om slimme, contextbewuste regels.  
- Manufacturing & supply chain: zelfs het beste ontwerp moet reproduceerbaar en schaalbaar zijn (Johnny Ive’s design to product gap).

# Conclusies en vooruitblik
- Technologie voor echt nuttige, realtime, persoonlijke AI-assistants is conceptueel in zicht: de benodigde wetenschappelijke ideeën (Bayes, Active Inference, neuromorphic efficiency) bestaan en er zijn proof-of-concepts (simulators, eye-tracking, adaptive HMI) die beloven.  
- Grote obstakels zijn engineering/energie, privacy & wetgeving, integratie-ecosystemen en vooral de juiste vormfactor die gebruikers bereid zijn dagelijks te dragen.  
- Tijdsinschatting deelnemers: mogelijk binnen 5–10 jaar reële adoptie van nieuwe devices/assistenten die on-device, realtime, gepersonaliseerd en privacybewust functioneren — maar onzekerheid over wanneer precies; veel hangt af van uitvoering, mode/acceptatie en supply chain.