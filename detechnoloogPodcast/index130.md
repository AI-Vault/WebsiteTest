# 130. Wie temt het wilde westen van onze digitale identiteit? (2025-10-30) [link](https://www.youtube.com/watch?v=lLVjn_hHDR8)


 # Hoofdonderwerp
Bespreking van identity wallets en de impact van eIDAS 2.0 op digitale identiteit in Europa — wat identity wallets zijn, welke rol Ver ID (SaaS-platform) speelt, technische standaarden, use cases, concurrentie, risico’s en adoptiebarrières.

# Belangrijke thema's
- eIDAS 2.0-wetgeving: verplichtingen voor acceptatie van toegelaten digitale wallets (deadline-uitgangspunten: wallet beschikbaar 2026, verplicht kunnen accepteren 2027).  
- Drie soorten wallets: commercieel, EUDI (toegelaten volgens ARF) en big tech (Apple/Google/Samsung).  
- Interoperabiliteit, trustlists en nationale uitvoeringsverschillen tussen lidstaten.  
- Privacy, security en cryptografie (HSM, qualified signing, post-quantum-kwesties).  
- Adoptiebarrières: gebrek aan noodzaak voor eindgebruikers, fragmentatie, compliance-complexiteit bij ontvangende partijen.  
- Marktrol van intermediairs: Ver ID positioneert zich als “payment service provider”-achtige connector tussen veel wallets en afnemers.

# Technische standaarden en regelgeving
- eIDAS 2.0 en ARF (Architectural Reference Framework): definiëren welke wallets als EUDI gelden, welke protocollen en minimale attributen vereist zijn.  
- Minimale verplichte PII-attribute (EUDI-wallets): voornaam, achternaam, geboortedatum en geboorteplaats. Extra attributen mogelijk, maar onduidelijkheden blijven bestaan.  
- Trustlists: elk EU-lidstaat regelt wie geregistreerde ontvangers zijn (wie mag attributen opvragen). Dit leidt tot 27 nationale trustlists en veel complexiteit.  
- W3C-achtige standaarden en OpenID Connect for Verifiable Presentations / Verifiable Credentials (issuance & presentations) worden genoemd als technologische basis.  
- Voor beveiliging en rechtsgeldigheid: HSM’s, qualified timestamp/signing providers, certificaatketens en private key management zijn essentieel.  
- Zero-knowledge proofs (ZKP): relevante techniek voor leeftijdscontrole en het beperken van gedeelde data (bewijs “ouder dan 18” zonder geboortedatum te delen).

# Ver ID: positionering, rol en werkwijze
- Ver ID is een SaaS-platform/connector: doel = één integratiepunt voor ontvangende partijen (banken, gemeenten, verzekeraars, PSP’s) om alle relevante identity wallets te ondersteunen. Analogie: Stripe voor identiteit.  
- Kernwaarden: technisch connectorwerk + sterke focus op compliance, risk management en wallet-assessments.  
- Wallet-assessment: controle van cryptografische suites, post-quantum readiness, welke attributen wallets bevatten, gebruikersaantallen en security-architectuur — alleen wallets die voldoen worden aangesloten.  
- Product & organisatie: ~15–16 medewerkers; ontwikkeling in Eindhoven, business & risk in Amsterdam; werken met ISO/NEN/DORA-achtige eisen.  
- Businessmodel: SaaS abonnementen (basis/professioneel/enterprise), met verschuiving mogelijk naar transactiemodel in de toekomst; pricing afhankelijk van transacties, wallets en attributen. Ver ID haalt ook een rol in onboarding naar nationale trustlists.

# Use cases met bijbehorende programma’s / technologieën
- Inloggen bij gemeentelijke websites: integratie met DigiD / NL-wallet / commerciële wallets. Programma’s: Keycloak (demo in 13 minuten), OpenID Connect for Verifiable Presentations. Ver ID biedt de connector en compliance-laag.  
- Bankonboarding / hypotheek / leasen: wallets (commercieel of EUDI) kunnen DUO-diploma’s, KVK-registraties en belastinggegevens bevatten. Voorbeeld wallets genoemd in de tekst: Dateper (commercieel voorbeeld), Yoti (VK), Signicat (Nordic). Ver ID koppelt deze wallets aan banken zodat alleen benodigde attributen gedeeld worden.  
- Autohuur (Hertz-voorbeeld): klant kiest wallet in UI, krijgt QR-code van verhuurder, scant in wallet en deelt slechts de gevraagde attributen (rijbewijs + geldigheid). Technisch flow: wallet-authenticatie + verifiable credential presentation via QR.  
- Fysieke legitimatie (politie / snelheidscontrole): vandaag nog grotendeels fysiek; wettelijk verplicht worden van acceptatie van digitale rijbewijzen per eIDAS-timelines (soms al beschikbaar in landen zoals Portugal / VS MDL).  
- Leeftijdscontrole (alcohol / sigaretten / pornosite- toegang): use case voor ZKP / leeftijdsproof; in VK heeft Yoti grote tractie dankzij online age-verification-eisen (Online Safety Act). Pornhub & soortgelijke sites moeten “highly effective” age-verification implementeren — wallets + ZKP zijn hiervoor relevante oplossingen.  
- Zorgdata & datakluizen: onderscheid tussen identity wallets (gestructureerde credentials) en datakluis (ongestructureerde documenten). Combinatie: wallet regelt toegang/consent, datakluis levert de zorgdocumenten. Ver ID ziet kansen in zorg, maar dataformaten/regelgeving maken dit complexer.  
- Webauthenticatie / social media: toekomstige mogelijkheid voor leeftijdsverificatie of gebruikersauthenticatie via wallets; frictie & businessmodel van platforms bepaalt adoptie.

# Concrete tools, protocollen en workflows genoemd
- Wallet-technologie: verifiable credentials (VC), verifiable presentations (VP), OpenID for VP.  
- Identity-platforms / wallets: genoemd of vergeleken: Yoti, Signicat, Trinsic, Dateper (veelvuldig genoemd), Digid/NL-wallet, commerciële bank-wallets (bankapps die identity-functies toevoegen). Ook big tech wallets (Apple/Google/Samsung) en Apple’s Digital Credentials API.  
- Identity connector / IdP tooling: Keycloak en vergelijkbare OAuth/OIDC-implementaties (Okta genoemd als vergelijk). Keycloak gebruikte men als voorbeeld van snelle integratie voor login flows.  
- Security-infrastructuur: HSMs, qualified signing/timestamping services, certificaatmanagement, private key management.  
- Wallet-assessment workflow (door Ver ID): downloaden/of in-labs testen, cryptografisch review, gebruikersevaluatie, compliance-checks, live integratie en monitoring.

# Concurrentie en marktstructuur
- Concurrenten genoemd: Signicat (Nordics), Animo Solutions (Nederlands), Liy (Duitsland?), Profisus (Zwitserland), Trinsic (VS). Veel spelers bouwen op nationaal of branche-niveau.  
- Marktgedrag: veel commerciële wallets zoeken businessmodel; moeilijk om geld te verdienen alleen via wallet-downloads. Veel wallets pivotten richting B2B-intermediaries of connectors.  
- Big tech: Apple/Google/Samsung kunnen grote marktaandelen veroveren (Apple Pay/Apple ID analogie). EU wil big tech niet dominant laten worden in eIDAS-context — maar technische en UX-voordelen van big tech blijven sterk.

# Risico’s, zorgen en ethische kwesties
- Privacy & centralisatie: sommige commerciële wallets houden data federated/centraal (niet altijd lokaal op toestel), wat privacyrisico’s verhoogt. EU wil dat Big Tech buiten de deur houdt voor gevoelige data, maar onduidelijkheden blijven.  
- Cowboy-wallets / slechte cryptografie: veel wallets bestaan; Ver ID voert strenge assessments uit om slechte aanbieders te weren omdat foutieve cryptografie of centraal onveilige opslag risico’s geeft.  
- Worldcoin / biometrie-controverse: Worldcoin (Sam Altman) als voorbeeld van wereldwijde iris-scanning met airdrops — aanzienlijke privacy- en ethical zorgen. AI-narratief: Worldcoin wordt genoemd in verband met “proof-of-humanity”-vraagstukken en AI-agents.  
- Implementatie- en operationele risico’s bij ontvangende partijen: compliance, retentiebeleid (hoe lang mag ontvanger attributen bewaren), auditing en bewijsvoering van juiste verificatie op een later moment.

# Marktadoptie en praktische barrières
- Gebruikersadoptie: weinig spoed of “aha”-moment bij consumenten; veel oplossingen voelen als “noodzakelijk kwaad” en hebben lage virale adoptie. Belangrijke triggers zijn wettelijke verplichtingen (Pornhub age checks, eIDAS-acceptatie) of tastbare gemakstoename (minder documenten/upload-verzoeken).  
- Ontvangers (banken, gemeenten, verzekeraars) staan veelal “afwachtend” vanwege compliance, interne governance en de behoefte aan gecertificeerde oplossingen. Sommige grote spelers onderzoeken “buy vs build” — open source specificaties bestaan, maar compliance/operations duwen naar inkopen van gespecialiseerde SaaS/connectors.  
- Nationale verschillen: lidstaten kunnen eigen aanvullende eisen hanteren (bv. Duitsland nuanceert ARF), wat interoperabiliteit bemoeilijkt.

# Business / organisatie van Ver ID
- Teamgrootte en structuur: circa 15–16 medewerkers; development in Eindhoven; business & risk in Amsterdam. Alles in-house gebouwd vanwege complexiteit/controlebehoefte.  
- Funding: eerdere funding rond ~€2M genoemd; in volgende ronde gesprekken lopende.  
- Focus komende jaar: prioriteit op eenvoudige, direct bruikbare use cases (inloggen/authenticatie) en vervolgens uitbreiden naar complexere cases; samenwerken met grote integrators en systeemleveranciers om gemeenten/banken te bereiken.

# Nieuwe tools, AI-workflows en AI-nieuws genoemd
- Nieuwe/aanstaande tools & APIs:
  - Digital Credentials API van big tech (Apple et al.) om wallet-detectie en credential-presentatie te vergemakkelijken in webflows.  
  - OpenID Connect for Verifiable Presentations en W3C Verifiable Credentials/Presentations als onderliggende standaarden.  
  - Keycloak (open source) als voorbeeld van snelle integratie voor authentication flows.  
- AI-workflows & nieuws:
  - Worldcoin (project van Sam Altman): iris-scans + airdrops; AI-kant: discussie dat proof-of-humanity noodzakelijk kan zijn voor AI-agents — privacyrisico’s. Wordt kritisch besproken qua centrale opslag en databeheer.  
  - Algemeen AI-opmerkingen: verwijzing naar AI-agents die zich online voordoen en hiermee de relevantie van betrouwbare proof-of-humanity/identity vergroten. Geen concrete nieuwe AI-productlanceringen buiten Worldcoin genoemd.

# Aanbevelingen en aandachtspunten voor organisaties
- Begin met low-friction use cases (inloggen via wallet) om ervaring en vertrouwen op te bouwen, daarna complexere claims (diploma’s, zorgdata) implementeren.  
- Voer strikt wallet-assessment / cryptografische audits uit vóór acceptatie; eis HSM en qualified signing waar nodig.  
- Houd retentiebeleid en audit-logica juridisch duidelijk: wat mag de ontvangende partij bewaren en hoe bewijs je later dat verificatie correct was?  
- Werk met grote integrators/system houses (gemeente-leveranciers, PSPs) om snelle opschaling te bereiken.  
- Volg national trustlist-developments en plan voor meervoudige trustlists/interoperabiliteit.

# Conclusie
Het gesprek benadrukt dat eIDAS 2.0 een fundamentele verandering brengt: veel meer digitale identiteitstransacties, verplichtingen voor acceptatie door ontvangende partijen en grote operationele en compliance-uitdagingen. Ver ID profileert zich als connector en compliance-layer tussen wallets en afnemers, met nadruk op security- en risk-assessment. Technisch zijn standards (VC/VP, OpenID for VP) grotendeels helder, maar governance (trustlists, nationale nuances) en adoptie vormen de grootste remmen. Privacy- en ethische kwesties (Worldcoin/biometrie, big tech) blijven onderwerp van debat.