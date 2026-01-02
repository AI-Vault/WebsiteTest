# 104. OpenAI neemt je muis over met Atlas-browser +  vibecoden is de democratisering van software + Cla... (2025-10-23) [link](undefined)


 # Hoofdonderwerp
Deze aflevering behandelt recente AI-ontwikkelingen en -discussies op het vlak van privacy, medische toepassingen, en software-ontwikkeling met AI-gebaseerde tools. Centraal staan OpenAI’s Atlas-browser met diepe geïntegreerde AI-kapabilities, een genomineerd model van DeepMind (op basis van Gemma) voor kankertherapie, Entropics cloud-vaardigheden voor modeltaken, en een diepgaand gesprek over vibecoding: wat werkt, wat niet, en welke rol senioriteit, governance en AI-vaardigheden spelen in moderne engineering.

# Belangrijkste thema’s
- AI-integratie in browsers en privacy/veiligheid: navigatorovername, hele browser als AI-omgeving, en implicaties voor data-inzamelingspraktijken.
- AI en biomedische innovatie: taalmodel-achtige omzetting van cellen naar tekst en laboratoriumresultaten die mogelijk nieuwe kankertherapieën openen.
- Nieuwe AI-workflows en infrastructuur: voorgedefinieerde “cloud skills” en een kunnen delen van AI-competenties tussen modellen en platforms.
- Verbeterde zoekervaringen met AI: semantisch begrip in consumentzoekopdrachten en betere suggesties op basis van context en data.
- Vibecode en software-ontwikkeling: snelle prototyping met AI-gegenereerde code, de balans tussen snelheid en technische debt, en de verschuiving van rollen (junior → senior, architectuur, governance).
- Drie golven van AI en de behoefte aan tooling: traditionele ML, de opkomst van generatieve AI, en de bijbehorende tooling, opschaling en monitoring.
- AI-geletterdheid en maatschappelijke impact: experimenteren, onderwijs en bewustwording over datawaarde, privacy en bedrijfsmodellen van Big Tech.
- Licenties en make-or-buy-dilemma: wanneer intern bouwen zinvol is en wanneer (grotere) leveranciers nodig zijn.

# Nieuwe tools en AI-workflows

- Atlas: chat GPT Atlas-browser
  - Wat het is: een browser die als wrapper rondom Chromium opereert en diep geïntegreerde OpenAI-modellen inschakelt (ombrellende “omnimodellen” die meekijken in de browser).
  - Belangrijkste kenmerken: cursor kan door AI worden overgenomen; browsen op een webshop kan bestuurd worden door AI; mogelijk toegang tot browsgeschiedenis en gedrag als gebruiker toestemming geeft.
  - Gebruiksscenario’s: aankopen doen via AI-gestuurde interactie; documenten lezen en samenvattingen ophalen; browselogboeken gebruiken om eerder bezochte tabbladen terug te halen.
  - Privacy en risico’s: grote privacyvragen over welke data naar OpenAI en derden stroomt; geanonimiseerde gedragingen kunnen worden verzameld om modellen te trainen; OS-niveau-toegang is beperkt voor niet-Apple/Microsoft/Google-omgevingen; waarschuwing om voorzichtig te zijn met het delen van browsedata.

- Gemma-gebaseerd model (DeepMind + Y University)
  - Wat het is: een taalmodel dat cellen omzet in tekst (sell-to-sentence) en deducies kan doen op moleculair niveau en weefselanalyse.
  - Belangrijkste kenmerken: model leert hoe cellen werken en kan voorspellen welke medicijncombinaties tumoren zichtbaarder maken voor het immuunsysteem.
  - Gebruiksscenario’s: voorspellen van medicijncombinaties die tumorcellen beter herkenbaar maken; laboratoriumvalidatie van deze combinaties (bijv. 50% verbetering in zichtbaarheid).
  - Belang: dit is innovatie op het snijvlak van AI en biomedisch onderzoek, mogelijk toekomstige therapeutische routes.

- Entropic cloud skills
  - Wat het is: een systeem van “cloud skills”—voorgegeneraliseerde, ingebouwde competenties voor AI-modellen die herkend en gedeeld kunnen worden.
  - Belangrijkste kenmerken: zowel ingebouwde vaardigheden (bv. gegenereerde PowerPoint) als door gebruikers toegevoegde vaardigheden (code, bedrijfsregels, Excel-formules); kan delen tussen modellen en platforms mogelijk maken.
  - Gebruiksscenario’s: op maat gemaakte competenties toevoegen aan basismodellen; een bibliotheek/skills shop voor AI-competenties; delen van oplossingen zoals code-snippets en bedrijfsprocessen.
  - Implicaties: potentieel ecosysteem van gedeelde AI-vaardigheden die interoperabel zijn tussen OpenAI, Google en andere aanbieders.

- AI-gedreven semantisch zoeken (Dept/DEPT-context)
  - Wat het is: semantische zoekmachines die betekenis en context begrijpen in plaats van alleen keywords te matchen.
  - Belangrijkste kenmerken: training op klantdata (zoekopdrachten, klikdata) en productdata; kan relaties leggen (bijv. “schuurmachine”, “schuurpapier”).
  - Gebruiksscenario’s: retailer die menselijke zoekopdrachten in natuurlijke taal begrijpt en relevante resultaten en slimme suggesties biedt; dagelijkse data-feed maakt het systeem slimmer.
  - Impact: betere conversie en klanttevredenheid door relevantere resultaten.

# Gebruiksscenario's en gebruikte programma’s

- Browsers en data-inzamelingen
  - Atlas als default browser; data over browsegedrag kan gebruikt worden om modellen beter te trainen; gebruikers waarschuwen voor privacy-implicaties.
- Klinisch-biomedisch onderzoek
  - Gemma-gebaseerd model zet cellen om naar zinnen en voorspelt medicijncombinaties; laboratoriumverificatie toont betere herkenning voor immuuncellen.
- Cloud-vaardigheden en workflow-ontwerp
  - Cloud skills creëren herbruikbare componenten (bijv. code, Excel-formules) die door AI-modellen kunnen worden toegepast en gedeeld tussen systemen.
- Zoekmachines en retail
  - Semantische zoekmodellen ingebouwd in een zoekfunctie; data-driven verbetering van relevante resultaten en slimme suggesties.
- Vibecode (interview met Judit van Steegeren)
  - Snelle prototyping via AI-gegenereerde code; bootstrapping van functionaliteit zoals webscrapers; later onderhoud en refactor door senior developers.
- Software engineering en AI-werkstromen
  - Logging en tracing van taalmodelgedrag; system prompts en prompt-ontwerp; afhankelijkheden en risk management (bv. afhankelijkheidscheckers zoals Dependabot).

# AI-gerelateerd nieuws (belangrijkste berichten uit deze aflevering)

- OpenAI introduceert Atlas: een browser waarin AI-gebaseerde controle over muis en sessies mogelijk is, met diepe integratie in Chromium.
- DeepMind (met Y University) werkt aan een Gemma-gebaseerd model dat cellen omzet naar tekst en medicijncombinaties voorspelt die tumoren zichtbaarder maken voor het immuunsysteem; laboratoriumtests tonen verbetering in herkenning.
- Entropic introduceert cloud skills: voorgedefinieerde AI-competenties en een bibliotheek waarmee bedrijven en modellen vaardigheden kunnen delen en uitbreiden, met praktische voorbeelden zoals automatisch gegenereerde PowerPoints en codeblocks.

# Impact op werk en organisatorische implicaties

- Vibecode en de arbeidspraktijk
  - Sneller prototyping, maar risico’s op fragmentarische, mogelijk onveilige code (gedogen door snelle markttoepassingen).
  - De rol van senior developers verschuift naar systeemarchitectuur, governance, en het saneren van technische debt; de behoefte aan logging en traceerbaarheid wordt groter.
  - Junioren krijgen minder kans om volledig te leren door lange opbouw in traditionele SDLC, waardoor mentoring en deliberate practice cruciaal blijven.
- Nieuwe rollen en vaardigheden
  - De benaming “machine learning engineer” blijft gangbaar voor generatieve AI-specialisten; prompt-engineer-achtige titels raken minder belangrijk naarmate tooling volwassen wordt.
  - Engineers moeten in staat zijn om AI-systemen te lezen, te controleren en te helpen bij menselijke-lus (human-in-the-loop) beslissingen, zeker bij kritieke toepassingen.
- Organisatorische keuzes: make-or-buy
  - Voor sommige AI-toepassingen is intern experimenteren mogelijk en waardevol; voor andere gevallen kan bedrijfstakken er beter aan doen om leveranciers te licenseren.
  - Het AI-veld is nog jong; leveranciersmarkt is onvolwassen. Organisaties moeten investeren in bewezen tooling en tegelijkertijd waakzaam blijven voor hype en oneerlijke beloften.

# Drie golven van AI en wat dit betekent voor tooling en werk

- Golf 1: traditionele machine learning en datawarehousing/operaties
  - Standaard tooling ontstaat: modellering, monitoring, data pipelines, en duidelijke rollen zoals data scientist.
- Golf 2: generieke AI en exogene AI-tools
  - Generatieve AI brengt nieuwe workflows en experimenten; tooling is vaak experimenteel en wispelturig.
- Golf 3: geïntegreerde AI-workflows en governance
  - Behoefte aan robuuste tooling om modelgedrag, betrouwbaarheid, veiligheid en interpretatie te borgen; human-in-the-loop en audit trails becomes essential.

# Belangrijke lessen en adviezen

- Experimenteer bewust
  - Stimuleer experimenteren met AI-tools, maar wel met common sense, vakkennis en kritische evaluatie van uitkomsten.
- AI-vaardigheden bouwen
  - Ontwikkel AI-geletterdheid op meerdere niveaus: digitaal, machine-learning geletterdheid en generatieve AI-geletterdheid; onderwijs en training spelen een sleutelrol.
- Transparantie en toezicht
  - Loggen, tracing, en duidelijke prompts/regels helpen om onzekerheden en ongewenst gedrag te beperken; system prompts en prompt-inzet moeten beheersbaar blijven.
- Human-in-the-loop en ethiek
  - Niet alles kan of moet door AI worden gedaan; human experts blijven cruciaal voor kwaliteitscontrole, domeinspecifieke kennis en veilige implementaties.
- Datawaarde en bedrijfsmodellen
  - Data blijft een kernwaarde (hoe mensen interacteren, wat ze lezen, hoe lang ze blijven); bedrijven moeten transparante, verantwoorde data-praktijken handhaven.

# Samenvatting van hoofdpunten
- Atlas toont een toekomst waarin AI meer en meer browser-omgevingen overneemt, met privacy- en data-flow-implicaties die zwaarder wegen naarmate AI-inzage toeneemt.
- Gemma-gebaseerde modellen openen een kans om cellen en medicijnen op een meertalig, tekst-achtige manier te koppelen aan new biomedical insight, met veelbelovende maar voorlopige laboratoriumresultaten.
- Cloud skills introduceren een mogelijk gedeelde bibliotheek van AI-competenties die tussen modellen en platforms kan circuleren, wat samenwerking en herbruikbaarheid vergroot.
- Vibecode illustreert snelheid en creativiteit bij prototyping, maar laat aanzienlijke zorgen achter op gebied van beveiliging, technische debt en rolveranderingen in engineering-teams.
- De drie golven van AI benadrukken dat tooling en processen sneller volwassen moeten worden; menselijk inzicht, governance en AI-vaardigheden blijven cruciaal.

Wil je dat ik deze samenvatting omzet in een compacte brief voor collega's of een presentatiewerkblad met punt-voor-puntuse-cases per tool?