# 108. AI-drones zijn nu al sneller dan de mens (2025-06-12) [link](https://www.youtube.com/watch?v=0hhGakHX3gs)


 # Hoofdtopic
Een Nederlandse podcastconversatie over autonome race‑drones: onderzoek van het Micro Air Vehicle Lab (TU Delft) dat autonome FPV‑drones ontwikkelde en daarmee een wereldwijde race in Abu Dhabi won. Focus ligt op technische ontwikkelingen (hardware en AI), toegepaste methodes (supervised learning + reinforcement learning), sim‑to‑real workflows (digital twins), praktische uitdagingen tijdens de competitie en maatschappelijke toepassingen (landbouw, inspectie, defensie, beveiliging).  

# Belangrijkste thema's
- Autonomie in drones: verschuiving van menselijke FPV‑besturing naar volledig boord‑AI.
- Snelle vooruitgang in motoren, aerodynamica en batterij/energie‑efficiëntie.
- AI‑architecturen: combinatie van supervised learning (poortdetectie) en reinforcement learning (vluchtbesturing).
- Sim‑to‑real transfer via digital twin en domain randomization.
- Hardware‑beperkingen en sensorsynchronisatie als bottlenecks (rolling shutter camera, IMU‑saturatie).
- Maatschappelijke toepassingen en ethische/veiligheidsvragen (landbouw, inspectie, defensie).
- Wetenschappelijke openbaarheid: publicatie en open source aankondiging.

# Technische aanpak en workflows
- Hardware-setup (competitie): identieke quadcopterframes, één enkele voorwaartse camera (rolling shutter), een Nvidia‑computer aan boord, inertiële sensors en motorcontrollers. Organisatie leverde exact dezelfde componenten aan alle teams — wedstrijd werd beslist op software.
- Perceptie (supervised learning):
  - Doel: herkennen en lokaliseren van gates/poortjes in verschillende belichtingscondities.
  - Workflow: datasetgeneratie (oefenbanen), hand‑labeling van gates, training van een detectie‑model. Model bleek goed te generaliseren naar andere hal/andere belichting.
- Besturing (reinforcement learning, RL):
  - Doel: leren van agressieve, snelle vlieglijnen en robuuste recovery bij fouten.
  - Workflow: RL wordt grotendeels in simulatie (digital twin) getraind met miljoenen iteraties; policies vervolgens op de echte drone ingezet.
  - Technische strategie: gebruik van een abstractielaag / low‑level controller op het echte platform (draaisnelheidscommando's) om sim‑to‑real gap te verkleinen.
- State estimation (sensorfusie + voorspelling):
  - Combinatie van visuele detecties (poortgrootte/positie), IMU‑meting en voorspellende dynamische modellen. Menselijke afstemming (tune van gewichten en vertrouwensregels) speelde grote rol.
- Sim‑to‑real technieken:
  - Digital twin met uitgebreide randomisatie: variatie in sensorruis, vertragingen, aerodynamica en belichting zodat getrainde controllers robuust zijn.
  - Hardware‑abstractie: in de simulator wordt commando‑niveau geabstraheerd (bijv. wheel/rotor speeds vs. motor PWM) om mismatch te minimaliseren.
- Iteratief afstellen live tijdens event:
  - Teams mochten tijdens de competitie calibreren/fine‑tunen; Delft schakelde tijdens de finale tussen verschillende RL‑policies (het beroemde “16.5‑seconden‑moment”) om snelheid en onverwachte vliegpatronen te benutten.

# Gebruikte tools en softwarecomponenten (specifiek en in context)
- Nvidia GPU / compute: trainings‑en inference‑workloads, simulatie‑acceleratie. Centrale rol in RL‑training en complexere perceptietaken.
- Simulator / Digital twin: ontwikkeld/gestandaardiseerd voor training van RL‑agents; bevat variaties in fysica en sensoren (domain randomization).
- Supervised learning frameworks (impliciet): datasets en handlabeling voor gate detection — modellen draaien real‑time op de Nvidia‑board.
- Reinforcement learning frameworks (impliciet): policy‑training met miljoenen episodes in sim; policies uitgevoerd als realtime controllers aan boord.
- Low‑level controller (regelaar): abstractielaag op drone die draaisnelheid/hoekposities aanhoudt en zo sim‑to‑real betrouwbaarheid verhoogt.
- Spiking neural networks (SNNs): onderzoeksrichting genoemd voor toekomstige extreem energiezuinige onboard inference (bio‑geïnspireerde neuronen).
- Data‑workflow: dataset creatie (oefencircuits), handlabeling, training, domain randomization, sim‑to‑real transfer en live tuning op locatie.

# Use cases en concrete toepassingen (met gebruikte programma's/technieken)
- Drone‑race/autonomie (competitietoepassing):
  - Programma/componenten: supervised gate detection + RL‑policy voor vlieggedrag; Nvidia compute voor training; digital twin voor simulatie.
  - Use case: autonome door‑poort‑races zonder menselijke piloot; benchmark voor algorithmedefinitie en robuustheid.
- Kassen (agri/greenhouse inspection) — “flappende” robots:
  - Programma/componenten: ontwerpen van bladvriendelijke airframes; lichte perceptie en navigatie‑AI; energiezuinige onbordcompute (eventueel SNNs).
  - Use case: veilig in kassen vliegen om planten te inspecteren zonder bladschade; autonome routines voor monitoring ziekte/stress.
- Maritieme inspectie / lange endurance inspectiedrones:
  - Programma/componenten: hybride designs (VTOL + efficiënte vleugel), planning‑algoritmen, energie‑beheer en lange‑afstand state estimation.
  - Use case: inspectie vanaf schepen, continue observatie, efficiëntie via aerodynamische optimalisatie.
- Industriële inspectie / logistieke kleine leveringen (voorbeelden zoals bezorgdrone voor bier genoemd als illustratie):
  - Programma/componenten: compacte detectie‑en‑navigatie stacks; veilige low‑power inference (SNNs) voor steeds kleinere platforms.
  - Use case: varen tussen mensen, binnenruimtes, last‑mile delivery in veiligheidsgevoelige omgevingen.
- Beveiliging / counter‑drone & defensie:
  - Programma/componenten: autonome detectie van ongewenste toestellen, interceptieplanners, mogelijke integratie met countermeasures.
  - Use case: detectie en neutralisatie van indringers; debat over ethische inzet blijft relevant. (Team werkt ook aan beschermingsmaatregelen.)

# Nieuwe tools / AI‑workflows uit het gesprek
- Digital twin als geïntegreerd ontwerpmiddel voor RL‑training: niet één realistische simulatie, maar een verzameling gesamplede omstandigheden (randomization) om generalisatie te vergroten.
- Combinatie‑workflow: supervised perceptie (poortherkenning) + RL‑gebaseerde policy voor hoog‑snelheidscontrole + state estimation die vision, IMU en voorspelling combineert — dit gecombineerde pad is de kern van hun aanpak.
- Abstractielaag/low‑level controller om sim‑to‑real gap te verkleinen: de RL bestuurt op een hoger niveau (draaisnelheden), echte hardware handelt low‑level actuatorcommando’s af.
- Live policy switching tijdens competitie: meerdere getrainde policies beschikbaar houden en tussenin overschakelen op basis van real‑time performance/risicomanagement.
- Spiking neural networks als onderzoekslijn voor ultra‑efficiënte onboard AI‑inference.

# Belangrijkste uitdagingen en beperkingen
- Hardwareimitaties van de organisatie: identieke, vaak goedkope sensoren (rolling shutter camera) en niet‑gesynchroniseerde sensorstreams. Deze beperkingen maken timing/synchronisatie kritieke factoren.
- Sensorlimieten: accelerometer‑saturatie bij hoge g’s, rolling shutter vervormingen bij snelle bewegingen, en vertragingen tussen camera frames (18 ms) die perceptie lastig maken.
- Sim‑to‑real mismatch: zonder degelijke digital twin en low‑level abstrahering is RL-training in sim nutteloos op de werkelijkheid.
- Regulatorische en maatschappelijke adoptie: operationele inzet (bv. kassen, landbouw) hangt af van regels, publieke acceptatie en certificatieprocedures.

# AI‑nieuws en maatschappelijke impact gemeld in het gesprek
- Wedstrijdresultaat en exposure: TU Delft won de autonome race en versloeg in finale zelfs de beste menselijke FPV‑piloten; een clip werd door Elon Musk geretweet wat veel aandacht veroorzaakte.
- Prijzengeld en competitiecontext: totale prijzenpot rond 1 miljoen USD; organisatie leverde gelijke hardware om software/AI te laten winnen.
- Wetenschappelijke follow‑up: Delft werkt aan publicatie en (gedeeltelijke) open‑source vrijgave van methoden.
- Kritische kanttekeningen bij gebruik in oorlogsvoering: er is debat over hoe veel AI er daadwerkelijk in conflictzones gebruikt wordt; veel huidige toepassingen in oorlogsvoering bevatten simpele autonome plannen en traditionele algoritmes, niet per se geavanceerde RL‑AI.
- Energie‑efficiëntie als belangrijke maatschappelijke thema: werk aan SNNs en energiezuinige AI kan grotere maatschappelijke impact hebben (minder energiegebruik in datacenters/edge devices).

# Concrete uitkomsten en highlights
- Technische doorbraak in competitie: eerste eerlijke vergelijking tussen mens en robot met beide één camera; Delft behaalde 17 s laps en later 16.5 s door live policy‑tuning (het “16.5‑moment”).
- Publicatie en open kennismaking: team kondigt paper en open uitleg aan; veel van de aanpak zal gepubliceerd worden.
- Bewijs dat gecombineerde AI‑workflows (supervised detection + RL + digital twin + predictieve state estimation) praktisch inzetbaar en competitief zijn op beperkte hardware.

# Volgende stappen, benodigdheden en onderzoeksvragen
- Opschaling: meer rekenkracht en betere simulators (grotere digital twins) versnellen training, maar Delft zoekt in de tussentijd slimme softwaretrucs om bij te benen zonder enorme investeringen.
- Samenwerking: behoefte aan partnerschappen rond energie‑efficiënte hardware en gespecialiseerde compute (defensie, industrie, industriële partners).
- Engineering uitdagingen: betere sensor‑synchronisatie, robuustere sensoren voor hoge g‑scenario’s, en verdere optimalisatie van weight/energy/compute trade‑offs.
- Regulering en implementatie: integreren in echte sectoren vraagt certificatie, regelgeving en maatschappelijke acceptatie (met name buiten competities).

# Conclusie / slotopmerking
Het gesprek laat zien hoe een praktisch, competitiegedreven onderzoeksproject complexe AI‑workflows integreert (supervised learning, reinforcement learning, digital twins, state estimation) om een autonome drone te bouwen die op beperkte hardware menselijke topprestaties kan evenaren en verslaan. Tegelijk benadrukt het de noodzaak van energiezuinige AI, robuuste sensorsynchronisatie en maatschappelijke/regelgevende aandacht bij opschaling naar reële toepassingen.