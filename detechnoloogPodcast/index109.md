# 109. AI-drones zijn nu al sneller dan de mens (2025-06-12) [link](https://www.youtube.com/watch?v=0hhGakHX3gs)


 # Technoloog 446 — Autonome racende drones, AI-workflows en toepassingen

Belangrijkste onderwerp en thema's
- Hoofdonderwerp: autonome FPV-racedrones bestuurd door AI die menselijke top-piloten verslaan tijdens een wedstrijd in Abu Dhabi.
- Kern­thema's: snelle ontwikkeling van dronehardware (motoren, propellers, batterijen), AI voor navigatie en besturing (supervised learning + reinforcement learning), state estimation en sensorfusie, digital twins/simulatie voor training, energie-efficiëntie en edge‑AI (spiking neural networks), ethiek/regulering en toepassingen (landbouw, kasinspectie, maritieme inspectie, defensie/counter‑drone).
- Belangrijke uitkomsten/nieuws: team van TU Delft won de autonome robotcompetitie en versloeg zelfs de beste menselijke FPV‑piloten; video van de overwinning kreeg aandacht (retweet door Elon Musk); prijzenpot van de competitie was ~1 miljoen USD; Delft publiceert en wil open source toelichten.

Evenement, uitslag en AI‑nieuws
- Wedstrijd: AORL x DCL-evenement in Abu Dhabi (grote indoorhal met poortjes/gates).
- Format: autonome drones (ieder team kreeg identieke hardware: quadcopter frame, Nvidia‑computer + één frontcamera, stuur‑/sensorbord) moesten zelfstandig het parcours doorvliegen; later gecombineerd met menselijke FPV‑piloten in finale.
- Nieuwswaardige punten:
  - TU Delft won de autonome competitie en in de gecombineerde finale versloeg de AI‑drone ook top menselijke piloten.
  - Video van Delft’s prestatie werd geretweet door Elon Musk — extra exposure en discussie rond AI‑veiligheid.
  - Organisatie stelde strenge eisen (geen meetapparatuur in de hal, identieke hardware voor alle teams), wat de vergelijking tussen teams eerlijke maakte.
  - TU Delft bereidt publicatie en open‑source materiaal voor over methoden en resultaten.

Technische ontwikkelingen sinds ~2007 (hardware vs. intelligentie)
- Hardwareverbeteringen:
  - Efficiëntere motoren en propellers, geoptimaliseerde airframes: veel hogere acceleratie en topsnelheden (geïllustreerd met voorbeelden van drones die auto’s volgen).
  - Beter batterij‑energy‑density en lichtere frames waardoor snel, acrobatisch vliegen mogelijk is.
  - Goedkopere, sterk verbeterde sensoren en camera’s (voortgang dankzij smartphone‑markt).
- Software/AI‑ontwikkelingen:
  - Traditionele FPV (mens bestuurt via bril) heeft weinig AI; signaal wordt draadloos gestuurd.
  - Moderne autonome systemen combineren computer vision, state estimation, predictive modeling en learning‑based control.
  - Kritische beperking: vaak niet de computervoordelen maar sensor‑limieten (rolling shutter camera artefacten, unsynchronized IMU/camera, accelerometer saturatie) bepalen prestaties.

AI‑architectuur en workflows (gedetailleerd)
- Data‑driehoek: supervised learning + reinforcement learning + klassieke regeltechniek (controller).
  - Supervised learning:
    - Doel: detectie/ herkenning van gates/poorten in de camerabeelden.
    - Workflow: dataset genereren (praktijkdata + augmentatie), hand‑labelen van gates, trainen van CNN‑achtige modellen op de Nvidia GPU.
    - Resultaat: betrouwbare gate‑detector die generaliseert naar andere hallen/condities (transfer zonder extra labeling).
  - Reinforcement learning (RL):
    - Doel: leren van agressieve, snelle vlieggedragingen en tactische inhaal‑/bochtstrategieën.
    - Workflow: trainen in een digital twin/simulator met enorme aantallen episodes; RL‑agent experimenteert, faalt veelvuldig en versterkt succesvolle gedragingen via reward‑functies.
    - Belangrijke facetten: reward‑engineering door mensen (menselijke feedback/tuning van rewardfunctie), gebruik van een goede digital twin om sim‑to‑real gap te verkleinen.
  - State estimation & sensorfusie:
    - Combineert visuele detecties (gates), IMU‑metingen en voorspellend model (motion model) om nauwkeurig positie/oriëntatie en bewegingsvector te schatten.
    - Extra element: voorspelling/‘memory’ — onthouden van recent gedrag om korte periodes zonder zicht te overbruggen (vergelijkbaar met menselijke pilotintuïtie).
  - Abstractielaag / low‑level controller:
    - In plaats van direct motorcommando’s sturen, stuurt de AI setpoints (draaisnelheden, lijngedrag) naar een onboard controller. Hierdoor wordt de digital twin‑modelklok betrouwbaarder en sim‑to‑real verschil kleiner.
- Simulator / digital twin:
  - Essentieel voor RL: agenten trainen miljoenen keren in simulatie i.p.v. onveilige real‑world crashes.
  - Domain randomization / variatie in simulatie‑parameters maakt modellen robuuster.
  - Digital twin moet nauwkeurig genoeg zijn (aerodynamica, sensorlatentie, rolling shutter effecten) — betere simulators vergen veel rekenkracht.
- Deploy workflow tijdens wedstrijd:
  - Start met conservatieve, betrouwbare mode (langzamere lap‑tijden, bijv. 30 s), verzamelt real‑world data, finaal finetunen en switch naar snellere/risicovollere policy (progressie naar 25s → 20s → 17s → 16.5s).
  - Model‑switching (één druk op de knop) wisselt tussen RL‑geoptimaliseerde vliegstrategieën, soms verrassend anders en moeilijk in te schatten voor menselijke tegenstanders.

Belangrijke hardware/engineering‑issues en beperkingen
- Camera‑eigenschappen: rolling shutter met 18 ms tussen eerste en laatste pixel; geometrische vervormingen bij snelle bewegingen.
- Sensor‑synchronisatie: camerafeeds en IMU‑data van verschillende fabrikanten moeten tijdsynchronisatie krijgen; milliseconde‑fouten leiden tot positioneringsfouten.
- Sensor saturatie: accelerometers bereiken meetlimieten tijdens hoge G‑manoeuvres → geven onjuiste waarden (klappen tegen mechanische aanslag), wat state estimation kan ontregelen.
- Wedstrijdconstraints: identieke hardware, verboden voor meetapparatuur in de hal, beperkte tijd voor afstelling → dwingt software‑robustheid en snelle iteratie.

Nieuwe tools, AI‑ideeën en technieken genoemd
- Digital twin / geavanceerde simulators (domain randomization, high fidelity physics) voor RL‑training.
- Reinforcement learning voor dynamische besturing en agressieve tactieken.
- Supervised learning voor gate detection (vision models).
- State estimation die combineert vision, IMU en predictieve component (fusion + memory‑achtige voorspelling).
- Abstractielaag (low‑level controller) om sim‑to‑real gap te verkleinen.
- Spiking neural networks (SNNs) en biologisch geïnspireerde neuronen:
  - Doel: drastische energie‑reductie op edge (potentieel 1000× zuiniger in sommige testgevallen).
  - Idee: alleen computation uitvoeren bij signaalverandering (sparse, event‑driven), ideaal voor always‑on camera’s of zeer beperkte payload drones.
- Traditionele controltechnieken genoemd: PID en INDI (nonlinear inversion control) — onderscheid tussen klassieke regeltechniek en learning‑based AI.

Gedetailleerde use cases + welke programma’s/technieken worden ingezet
- Drone‑racing (competities):
  - Programma/techniek: Nvidia GPU voor training/deployment, supervised CNN voor gate detectie, RL‑agent getraind in digital twin, state estimator (visual‑inertial fusion), abstracts controller voor robuuste motoraansturing.
  - Eigenschappen: real‑time inference aan boord, model‑switching voor verschillende snelheidsmodi, latency/sync‑management.
- Kasinspectie met flappende vleugelrobots:
  - Hardware: flapperende vleugels i.p.v. propellers (veilig voor planten).
  - Programma/techniek: autonome navigatie algoritmes + vision voor bladdetectie/ziekteherkenning; energiezuinige inferentie (eventueel SNN) voor langere inzet.
  - Waarom: fysiek veilig (botsen met bladeren) en lichtgewicht.
- Landbouw / crop monitoring:
  - Programma/techniek: vision‑based plant health detection (supervised learning), planning/coverage algorithms; lichte onboard inference voor kleine drones of offload naar edge servers voor grotere UAV’s.
  - Beperkingen: regelgeving, operationele workflows en kosteneffectiviteit voor boeren.
- Maritieme inspectie / offshore:
  - Hardware: hybride ontwerpen (VTOL + efficiënte vleugel) voor lange endurance en landingsmogelijkheden op muren/deksels.
  - Programma/techniek: lange‑term planning, GPS/visual fusion, energiebeheer.
- Bezorging / logistiek (klein schaal‑delivery):
  - Programma/techniek: autonome navigation & obstacle avoidance + SNNs/edge‑optimalisatie voor langere batterijduur.
- Counter‑drone / defensie‑toepassingen:
  - Programma/techniek: detectie/classificatie via vision + autonomous interception planning; TU Delft benadrukt ook onderzoek naar defensieve toepassingen en bescherming tegen ongewenste drones.
  - Opmerking: veel operationele systemen in conflictgebieden maken nog veel gebruik van meer traditionele geprogrammeerde strategieën; echte learning‑based autonomie is nog niet universeel toegepast.
- Energy‑efficient AI op edge:
  - Programma/techniek: spiking neural networks, event‑cameras, sparse inference, hardware‑aware model design om AI op kleine drones mogelijk te maken.

Regulering, ethiek en maatschappelijke aspecten
- Veiligheid en regelgeving beperken snelle opschaling (ruimtelijke ordening van drones in civiele luchtvaart vereist streng bewijs van veiligheid).
- Dual‑use dilemma: dezelfde technieken voor maatschappelijke toepassingen (agri, inspectie, search & rescue) kunnen ook voor militaire doeleinden toegepast worden.
- TU Delft‑houding: expliciete aandacht voor energie‑efficiënte AI, maatschappelijk nuttige toepassingen en verantwoord gebruik; actieve discussie over defensie‑overlap.

Beperkingen, uitdagingen en benodigde resources
- Beperkingen van small‑form‑factor hardware (sensors, compute en power) blijven de bottleneck.
- Synchonisatie van heterogene sensoren en rolling shutter artefacten vereisen slimme algoritmische compensatie.
- Simulators/digital twins van hoge kwaliteit zijn rekenintensief — grote teams of cloud/GPU‑resources versnellen ontwikkeling (maar zijn duur).
- Voor verdere stappen zijn samenwerking, funding en teams (PhD’s, MSc’s, stagiaires) cruciaal — TU Delft zoekt vervolgteams en samenwerkingen.

Vervolgstappen en publicatie/open‑source plannen
- TU Delft werkt aan een wetenschappelijke publicatie en wil methoden (algoritmes, state estimation technieken, simulatie‑aanpak) openbaar maken (open source).
- Verdere wedstrijden en races ingepland; iteratieve verbetering van simulators en RL‑workflows.
- Aandacht voor energiezuinige AI (SNNs) en toepassingen die direct maatschappelijk nut hebben (kassen, maritiem, inspectie).

Kort overzicht van technische lessons learned (praktisch)
- Forceer geen zwaardere hardware als de taak efficiënter met softwareoplossingen kan; optimalisatie van software en controlearchitectuur kan veel winnen.
- Gebruik digital twins + domain randomization voor RL‑training, maar zorg dat low‑level controllers abstraheren voor robuuste sim‑to‑real transfer.
- Combineer supervised vision voor object/gate detectie met RL voor dynamisch gedrag — beide vullen elkaar aan.
- Sensor synchronisatie en omgaan met sensorlimieten (accelerometer saturatie, rolling shutter) zijn kritieke engineeringdoelen voor hoge‑snelheids autonome vlucht.
- Plan voor model‑switching en veilige fallback‑modes tijdens competitie/operaties.

Conclusie
- De race in Abu Dhabi toont dat learning‑based autonome drones met beperkte sensoren (één camera + onboard compute) op competitief niveau snelle en robuuste vliegstrategieën kunnen leren en zelfs topmenselijke piloten kunnen verslaan.
- De gebruikte AI‑workflows combineren supervised learning (visie), reinforcement learning (gedragsoptimalisatie), nauwkeurige state estimation en een digital twin‑gedreven trainingspipe; spiking neural networks beloven significante energiewinst voor edge‑gebruik.
- Toepassingen reiken van landbouw en inspectie tot beveiliging en defensie; maatschappelijke adoptie vraagt naast technische vooruitgang vooral regelgeving, veiligheid en verantwoord gebruik.