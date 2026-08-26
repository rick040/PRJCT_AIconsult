# PRJCT AI — Basisframework

**Versie 1.2 · 25-08-2026 · Rick van Mierlo · Eindhoven/Geldrop**
Status: fundament. Elk hoofdstuk is bedoeld als losse werkmodule die later verder wordt uitgewerkt (eigen agent, eigen skill, eigen deliverable).

---

## 0. Executive summary

Nederlandse MKB-bedrijven met 10–25 medewerkers zetten elke AI-knop aan die hun software aanbiedt, zien er weinig van terugkomen en concluderen dat AI niet werkt. Het probleem zit niet in de knoppen maar in de laag eronder: rommelige bestandsstructuren, ongedefinieerde processen, kennis in hoofden en mailboxen, geen eigenaarschap. AI kan daar niets mee.

PRJCT AI zet die laag eerst neer — domeinen, workflows, mappen, naamgeving, bronwaarheid, kennisbestanden per domein — en bouwt daarna pas de AI-werkplek erop: skills, plugins, MCP-koppelingen naar hun eigen systemen, plus training zodat het team het zelf blijft gebruiken. Het resultaat is persoonsonafhankelijk en toekomstvast: elke volgende AI, elk nieuw document en elke nieuwe medewerker sluit direct aan.

Kern: **eerst structureren, dan inbouwen, dan overdragen.** Verkoopmotor: webinars en scans die doorlopen naar fundament, toolkit-sprints en retainers.

Doel: €10.000 omzet in 3 maanden uit deze lijn, zonder de bestaande design/web-omzet te vervangen.

---

## 1. Het idee

### 1.1 Wat het is
Een implementatie- en trainingspraktijk voor AI op de werkvloer. Geen losse chatbot-demo, maar een ingerichte AI-omgeving die past op hoe het bedrijf werkt.

### 1.2 Wat er concreet wordt opgeleverd
0. **Bedrijfsfundament** — de laag onder alle AI. Domeinen afgebakend (sales, operations, marketing, finance, HR), processen beschreven, eigenaarschap belegd, bestands- en mappenstructuur opnieuw ingericht, naamgevingsconventies vastgelegd, bronwaarheid per gegeven bepaald. Zo weet elke AI, elke MCP en elke nieuwe medewerker direct waar wat staat en wat ermee moet gebeuren — ook bij nieuwe documenten en bij een rolwissel.
1. **Skills** — herbruikbare, vastgelegde werkinstructies voor terugkerende taken (offerte maken, mail beantwoorden, rapport samenvatten, werkbon uitwerken).
2. **MD-bestanden / kennisbasis** — bedrijfscontext, tone of voice, prijzen, procedures, klanttypes, vastgelegd zodat elk AI-antwoord klopt met hun werkelijkheid.
3. **Plugins & toolkits** — een gebundelde set per afdeling, installeerbaar, met documentatie.
4. **MCP-koppelingen** — AI verbonden met hun echte systemen: mail, agenda, Drive/SharePoint, CRM, boekhouding, projecttool.
5. **Automatiseringen (n8n)** — voor wat volledig zonder mens moet lopen.
6. **Training & webinars** — live sessies per afdeling, plus opname en naslag.
7. **Governance-basis** — wat mag wel/niet in AI, AVG-afspraken, welke data waar.
8. **Lokale AI (add-on, in ontwikkeling)** — AI die op eigen hardware of eigen server draait in plaats van in de cloud. Zie 1.5.

### 1.3 Het lagenmodel — de kern van de aanpak

Ondernemers zetten elke AI-knop aan die hun software aanbiedt en concluderen daarna dat AI niet werkt. Dat klopt ook: die knoppen werken alleen zo goed als de structuur eronder. Een AI-functie in hun CRM kan niets met een klantdossier dat half in de mail zit, half in een map `Nieuwe map (3)` en half in het hoofd van één collega.

| Laag | Wat | Zonder deze laag |
|---|---|---|
| **0. Structuur** | domeinen, processen, eigenaarschap, mappen, naamgeving, bronwaarheid | AI raadt, en raadt fout |
| **1. Context** | MD-kennisbestanden per domein: prijzen, tone of voice, procedures, klanttypes | output klopt niet met hun werkelijkheid |
| **2. Werkinstructies** | skills per terugkerende taak | iedereen prompt anders, kwaliteit wisselt |
| **3. Koppelingen** | MCP en n8n naar mail, Drive, CRM, boekhouding | knippen en plakken blijft |
| **4. Borging** | training, champion, governance, onderhoud | dood na twee maanden |

**Regel: nooit een laag overslaan.** Wie bij laag 3 begint, bouwt automatisering op drijfzand. Laag 0 en 1 zijn het echte werk en het echte onderscheid. Laag 2 tot 4 zijn de zichtbare oplevering.

Bijkomend effect van laag 0: de structuur is toekomstvast. Nieuwe documenten landen op de juiste plek, een nieuwe medewerker of een nieuw AI-model pakt het direct op, en elke volgende tool die ze kopen werkt beter omdat de basis klopt.

### 1.4 Wat het niet is
Geen strategierapport. Geen enterprise-transformatietraject. Geen eigen SaaS-product. Geen tooling die alleen bij Rick werkt.

### 1.5 Lokale AI — toekomstige add-on, nog niet verkopen

**Status: verkenning. Niet actief aanbieden tot Rick zich heeft ingelezen en één werkende opstelling heeft gedraaid.** Wel meenemen in het framework, want het past logisch op het fundament en is later een sterke uitbreiding.

**Het idee.** Alle of een deel van de AI die het bedrijf gebruikt lokaal laten draaien: op eigen hardware of een eigen server, in plaats van bij een cloudleverancier. Bedrijfsdata verlaat het pand niet.

**Waarom dit later goed past.** Het fundament (laag 0 en 1) is modelonafhankelijk. Wie zijn structuur en kennisbestanden op orde heeft, kan het onderliggende model vervangen zonder opnieuw te beginnen. Lokale AI is dan een schakelaar, geen nieuw project. Dat is precies het argument waarmee het fundament nóg beter verkoopt: **"we bouwen dit zo dat je later kunt overstappen naar AI die volledig binnen je eigen muren draait."**

**Wie het wil.** Zorgpraktijken, accountants en advocatenkantoren met gevoelige dossiers; bedrijven met eigen ontwikkeling of technische IP; klanten die op AVG of AI Act vastlopen bij hun compliance-vraag; en directeuren met principiële bezwaren tegen data-in-de-cloud.

**Positionering:** premium add-on, geen instapproduct. Indicatie voor later: eenmalige inrichting €2.500 – €6.000 plus hardware, met een verhoogde retainer voor onderhoud. Prijzen pas vastzetten na de eerste eigen proefopstelling.

**Wat Rick eerst moet doen (geen klantwerk):** één lokale opstelling draaien op eigen hardware, meten wat er realistisch op draait, uitzoeken hoe MCP-koppelingen en de bestaande skills zich lokaal gedragen, en bepalen waar de grens ligt tussen "lokaal genoeg" en "hier is de cloud gewoon beter". Pas daarna een aanbod formuleren.

**Voorlopige lijn richting klanten:** wel benoemen als richting ("dit fundament is er klaar voor"), niet verkopen als dienst. Nooit toezeggen wat nog niet is uitgeprobeerd.

### 1.6 Businessmodel
Ladder van laag risico naar hoge waarde:

| Trede | Vorm | Functie |
|---|---|---|
| 0 | Gratis webinar / kennissessie | leadgeneratie, autoriteit |
| 1 | AI Readiness Scan | betaalde kennismaking, diagnose |
| 2 | Bedrijfsfundament | structuur op orde, verplichte basis |
| 2b | Toolkit Sprint (1 afdeling) | eerste zichtbare oplevering |
| 3 | Bedrijfsbreed traject | hoofdomzet |
| 4 | AI-partner retainer | terugkerende omzet, in gradaties — zie 8.5 |
| 5 | Toolkit-licenties / open trainingen | schaalbaar, arbeidsarm |

Merkkeuze: opereren onder **PRJCT AI** als aparte lijn binnen PRJCT Agency. Design/web blijft eigen ingang, maar levert wel cross-sell.

---

## 2. Doelgroepanalyse

### 2.1 Primair segment
- **Grootte:** 10–25 medewerkers (sweet spot 15–22)
- **Omzet:** €1M–€5M
- **Regio:** Eindhoven, Geldrop, Helmond, Veldhoven, Best, Nuenen, Son, Valkenswaard (Brainport)
- **Beslisstructuur:** 1–2 beslissers, DGA of MT-lid. Korte lijnen, beslissing binnen 2–4 weken.
- **IT:** externe IT-partner, Microsoft 365 of Google Workspace, geen eigen dev-capaciteit
- **Kenmerk:** te groot om nog "alles zelf even te doen", te klein voor een interne AI-afdeling

### 2.2 Meest kansrijke branches (in volgorde van prioriteit)

| Prio | Branche | Waarom raak |
|---|---|---|
| 1 | Zakelijke dienstverlening (accountants, adviesbureaus, makelaars, HR/recruitment) | veel tekst, veel dossiers, direct meetbare tijdwinst |
| 2 | Bouw, installatie, technische dienstverlening | veel offertes, werkbonnen, mailverkeer, personeelskrapte |
| 3 | Groothandel & productie-MKB | veel repetitieve administratie en klantcommunicatie |
| 4 | Zorgpraktijken / paramedisch (10–25 fte) | verslaglegging en administratielast, wel AVG-zwaar |
| 5 | Marketing-/mediabureaus | snelle adoptie, maar prijsgevoelig en doen veel zelf |

### 2.3 Uitsluiten (voorlopig)
< 10 medewerkers (geen budget, geen structuur), > 50 medewerkers (inkoopproces, security-audits, concurrentie van grote partijen), pure e-commerce (ander speelveld).

### 2.4 Marktomvang, ruwe schatting
Brainport-regio telt naar schatting enkele duizenden bedrijven in de klasse 10–50 medewerkers. Bij een bereikbaar deel van ~600 bedrijven in de prioriteitsbranches en een realistische conversie van 1–2% naar een eerste traject: 6–12 klanten per jaar bij één operator. Dat is ruim voldoende voor de doelstelling. **Actie: dit valideren met KvK-/Company.info-data voordat er hard op gestuurd wordt.**

### 2.5 Koopmoment (triggers)
- Personeelstekort of vertrek van een administratieve kracht
- Nieuwe jaarplannen (sep–nov, jan)
- Concurrent die zichtbaar met AI adverteert
- Mislukt eigen AI-experiment ("we hebben ChatGPT wel, maar niemand gebruikt het")
- Nieuwe MT'er of bedrijfsopvolging
- Subsidie-/opleidingsbudget dat op moet (SLIM-regeling, O&O-fondsen)

---

## 3. Persona's

### Persona 1 — Bas, de eigenaar (primaire beslisser)
**48, DGA installatie-/bouwbedrijf, 18 medewerkers, Helmond.**
Praktisch, wantrouwt hype, rekent in uren en euro's. Werkt zelf mee in de zaak. Beslist alleen, snel, als hij het snapt.

- **Doel:** meer werk aankunnen zonder extra kantoorpersoneel
- **Pijn:** offertes en mail blijven liggen, hij doet ze 's avonds zelf
- **Bezwaar:** "Kost dit me straks meer tijd dan het oplevert?"
- **Wint hem:** één concreet voorbeeld uit zijn eigen branche, met uren en bedragen
- **Verliest hem:** jargon, slides, "AI-transformatie", vaag uurtarief
- **Waar bereikbaar:** LinkedIn, ondernemersverenigingen, brancheavonden, via boekhouder/IT-partner

### Persona 2 — Marloes, de operationeel manager (initiatiefnemer + gebruiker)
**35, operations/office manager bij adviesbureau, 22 medewerkers, Eindhoven.**
Regelt alles, voelt de werkdruk het scherpst, heeft geen tekenbevoegdheid maar wél de doorslaggevende stem.

- **Doel:** processen soepel houden, team ontlasten, zelf niet het knelpunt zijn
- **Pijn:** iedereen prutst met een eigen AI-tool, niets is vastgelegd, kwaliteit wisselt
- **Bezwaar:** "Gaat mijn team dit echt gebruiken?"
- **Wint haar:** kant-en-klare werkinstructies, training, iets wat ze zelf kan beheren
- **Verliest haar:** een oplossing die alleen de consultant kan onderhouden
- **Waar bereikbaar:** LinkedIn, webinars, nieuwsbrief, vakgroepen

### Persona 3 — Joris, de interne AI-enthousiasteling (champion, geen budget)
**29, junior/medior, doet AI "erbij".**
Heeft al wat gebouwd, loopt vast op integratie en op collega's die niet meegaan.

- **Doel:** serieus genomen worden, zijn werk opgeschaald zien
- **Pijn:** heeft geen mandaat, geen tijd, geen structuur
- **Rol in de deal:** interne aanjager en later beheerder van de toolkit
- **Wint hem:** hem eigenaar maken van de toolkit, niet passeren
- **Waar bereikbaar:** LinkedIn, meetups, technische content

**Regel:** Marloes of Joris opent de deur, Bas tekent. Verkoopmateriaal moet voor beide werken: één businesspagina voor Bas, één praktijkpagina voor Marloes/Joris.

---

## 4. Probleem–oplossing fit

| # | Probleem (in hun woorden) | Onderliggende oorzaak | PRJCT AI-oplossing | Bewijs dat het werkt |
|---|---|---|---|---|
| 1 | "We weten niet waar we moeten beginnen" | geen zicht op eigen processen, te veel opties | AI Readiness Scan met geprioriteerde roadmap | roadmap met 5 use-cases, uren en euro's per stuk |
| 2 | "We hebben ChatGPT, maar niemand gebruikt het" | geen instructies, geen context, geen eigenaar | Skills + MD-kennisbasis + interne champion | gebruikscijfers na 30 dagen |
| 3 | "De uitkomst klopt niet met hoe wij werken" | AI kent hun prijzen, klanten, procedures niet | MD-kennisbasis en bedrijfscontext vastgelegd | output naast een handmatig voorbeeld leggen |
| 4 | "Alles staat los van onze systemen" | geen koppeling met mail, CRM, Drive | MCP-koppelingen + n8n | AI die hun eigen dossier ophaalt tijdens demo |
| 5 | "Mag dit wel met onze klantgegevens?" | AVG-onzekerheid | governance-basis + tool-/datakeuze | 1 A4 AI-gebruiksbeleid |
| 6 | "Elke medewerker doet maar wat" | geen standaard, geen borging | toolkit per afdeling + training + naslag | iedereen werkt vanuit dezelfde skills |
| 7 | "Het bloedt na twee maanden dood" | geen onderhoud, geen doorontwikkeling | retainer met kwartaalupdate, in gradaties (zie 8.5) | verlengingspercentage |
| 8 | "We hebben overal de AI-knoppen aangezet, maar het levert niks op" | ingebouwde AI-functies vinden geen bruikbare structuur en context | laag 0 en 1: structuur, mappen, eigenaarschap, kennisbestanden | dezelfde AI-knop naast elkaar, vóór en ná het fundament |
| 9 | "Als Jan weggaat, weet niemand meer hoe het zit" | kennis zit in hoofden en mailboxen, niet in het systeem | vastgelegde domeinen, procesbeschrijvingen, bronwaarheid | nieuwe medewerker werkt binnen een dag mee |
| 10 | "Elk nieuw document is weer improviseren" | geen naamgeving, geen vaste plek, geen conventie | structuurafspraken die AI en mens allebei volgen | nieuw document is binnen 5 seconden vindbaar en bruikbaar |

**Fit-conclusie:** de scherpste pijn is nummer 1 en 2. Daar hangt de instap aan op. Nummer 8 is de scherpste *bewijs*-pijn: bijna elke prospect heeft die knoppen al aangezet en is teleurgesteld, en dat is precies het gat waar het fundament in past. Nummer 3 en 4 leveren het wow-moment dat de sprint verkoopt. Nummer 7, 9 en 10 verkopen de retainer en het bedrijfsbrede traject.

---

## 5. Value proposition

### 5.1 Kernbelofte
> **AI werkt pas als je bedrijf erop is gebouwd. Wij zetten eerst de structuur neer — domeinen, workflows, bestanden, kennis, eigenaarschap — en bouwen daar de AI-werkplek bovenop. Resultaat: elke AI-functie die je nu of later aanzet, weet meteen wat te doen.**

Tweede regel, voor wie snel resultaat wil horen: *binnen 30 dagen werkt je team er echt mee, met vastgelegde werkinstructies, gekoppeld aan jullie eigen systemen, en training zodat het blijft hangen.*

### 5.2 Value Proposition Canvas (samengevat)

**Customer jobs:** meer werk aankunnen met hetzelfde team · administratie wegwerken · kwaliteit gelijk houden · niet achterlopen op concurrenten · geen geld verbranden aan hype

**Pains:** keuzestress · mislukte pilots · geen tijd om het uit te zoeken · AVG-angst · afhankelijk worden van een externe partij

**Gains:** uren terug per week · consistente output · team dat zelf verder kan · aantoonbaar voorlopen in de regio

**Pain relievers:** geprioriteerde roadmap in plaats van 40 opties · vaste prijs per fase · toolkit die zij bezitten · duidelijke datagrenzen

**Gain creators:** skills per rol · koppeling met eigen systemen · training + naslag · kwartaalupdate

### 5.3 Positioneringszin
Voor MKB-directies in Brainport met 10–25 medewerkers die AI willen invoeren maar door de bomen het bos niet zien, is PRJCT AI de partner die eerst hun bedrijf zo structureert dat AI er iets mee kan, en die AI daarna in het dagelijkse werk inbouwt en overdraagt — anders dan adviesbureaus die alleen een rapport achterlaten, of softwareleveranciers die een AI-knop leveren zonder dat er iets bruikbaars onder ligt.

### 5.4 Boodschap per persona
- **Bas:** "Twee dagen kantoorwerk per week terug, zonder extra personeel. En als Jan weggaat, ligt alles vast."
- **Marloes:** "Je team werkt vanaf dag één vanuit dezelfde vastgelegde werkwijze, en elk nieuw document landt vanzelf op de juiste plek."
- **Joris:** "Jij wordt eigenaar van een fundament waar elke volgende AI die jullie aanzetten meteen op werkt."

---

## 6. USP's

1. **Wij werken aan de laag onder AI.** Niet de knoppen, maar de structuur eronder: hoe het bedrijf is ingedeeld, hoe workflows lopen, waar bestanden staan, waar de bronwaarheid ligt, wie waarvan eigenaar is. Iedereen kan een AI-functie aanzetten. Wij zorgen dat die functie iets zinnigs aantreft. **Dit is de hoofd-USP — alle andere volgen hieruit.**
2. **Toekomstvast en persoonsonafhankelijk.** De structuur is zo opgezet dat nieuwe documenten vanzelf op hun plek landen, een nieuwe medewerker in dezelfde dag meedraait, en elke volgende AI of MCP direct weet wat te doen. Niet gebouwd voor het model van vandaag.
3. **Implementatie, geen advies.** Er wordt gebouwd, niet gepresenteerd. Elke fase eindigt met iets dat draait.
4. **Toolkit in eigendom van de klant.** Skills, MD-bestanden en documentatie blijven van hen, ook zonder PRJCT AI.
5. **Gekoppeld aan hun echte systemen.** MCP en n8n richting mail, Drive, CRM, boekhouding. Niet "chatten in een leeg venster".
6. **Vaste prijzen per fase.** Geen open uurtjes. Vooraf duidelijk wat het kost en wat eruit komt.
7. **Ontwerpachtergrond.** Materiaal, documentatie en training zijn verzorgd en begrijpelijk, niet een technische dump.
8. **Regionaal en fysiek aanwezig.** Langskomen, meekijken op de werkvloer, gezicht kennen.
9. **Één aanspreekpunt.** Geen accountmanager, junior consultant en projectleider — dezelfde persoon van scan tot borging.
10. **Adoptie ingebouwd.** Training, interne champion en 30-dagen-check horen standaard bij de levering.

**Pitchzin die USP 1 en 2 samenvat:** "Elke AI-knop in jullie software werkt precies zo goed als de rommel eronder. Wij ruimen die eerst op, en zetten er dan pas AI op."

**Bewijslast (te bouwen, prioriteit hoog):** 2 casussen met cijfers, 3 videodemo's van een echte skill, 1 publieke toolkit als proefmonster.

---

## 7. Product-market fit

### 7.1 Hypothese
MKB-bedrijven van 10–25 medewerkers in Brainport betalen €2.500–€10.000 voor een AI-implementatie mét training, wanneer die is gekoppeld aan hun eigen systemen en resulteert in aantoonbare tijdwinst binnen 30 dagen.

### 7.2 Validatiepad (12 weken)

| Fase | Weken | Doel | Slaagcriterium |
|---|---|---|---|
| A. Probleemvalidatie | 1–3 | 15 gesprekken met doelgroep | ≥ 10 noemen spontaan "weet niet waar te beginnen" |
| B. Aanbodvalidatie | 3–5 | scan aanbieden aan 15 leads | ≥ 3 betalen voor een scan |
| C. Leveringsvalidatie | 5–9 | 2 toolkit-sprints uitvoeren | ≥ 1 gemeten besparing van ≥ 4 uur/week |
| D. Herhaalvalidatie | 9–12 | retainer aanbieden aan sprintklanten | ≥ 1 tekent retainer |

### 7.3 PMF-signalen
**Groen:** klanten vragen zelf om uitbreiding naar een tweede afdeling · doorverwijzing zonder erom te vragen · scan wordt binnen 2 weken zonder korting geaccepteerd · gebruik na 60 dagen nog boven 60%
**Rood:** koper alleen op prijs · toolkit ongebruikt na 30 dagen · scan levert geen vervolg · elke klant vraagt iets totaal anders (= geen herhaalbaar product)

### 7.4 Meetpunten
Scan → sprint conversie (doel ≥ 50%) · sprint → retainer conversie (doel ≥ 40%) · gebruik na 30 en 60 dagen · gemeten uurbesparing per klant · NPS na oplevering

---

## 8. Pricing

### 8.1 Prijskaart

| Product | Prijs | Inhoud | Doorlooptijd |
|---|---|---|---|
| **Webinar / kennissessie (open)** | gratis of €49 p.p. | 60–75 min, live, met werkvoorbeelden | 1 dagdeel |
| **In-company workshop** | €950 per dagdeel | tot 15 deelnemers, praktijkgericht, incl. naslag | 1 dagdeel |
| **AI Readiness Scan** | €750 | procesinventarisatie, 5 geprioriteerde use-cases, roadmap, businesscase | 1–2 weken |
| **Bedrijfsfundament** | €2.500 – €5.000 | domeinindeling, procesbeschrijvingen, eigenaarschap, mappen- en naamgevingsstructuur, bronwaarheid, MD-kennisbasis per domein | 3–5 weken |
| **Toolkit Sprint (1 afdeling)** | €2.500 – €4.500 | 3–6 skills, MD-kennisbasis, 1–2 koppelingen, 2 trainingen, documentatie | 3–4 weken |
| **Bedrijfsbreed traject** | €7.500 – €15.000 | 3 afdelingen, koppelingen, governance, champion-opleiding, borging | 8–12 weken |
| **AI-partner retainer** | €99 – €2.000 p/m, in 4 gradaties | onderhoud, nieuwe skills, helpdesk, kwartaalupdate — zie 8.5 voor de volledige ladder | doorlopend |
| **Losse automatisering (n8n)** | €750 – €2.500 | per workflow, inclusief oplevering en documentatie | 1–2 weken |
| **Toolkit-licentie (branchepakket)** | €350 – €950 | kant-en-klaar pakket, zelf te installeren | direct |
| **Lokale AI-opstelling** *(nog niet verkopen)* | indicatie €2.500 – €6.000 + hardware | AI op eigen server/hardware, data blijft binnen. Prijs pas vast na eigen proefopstelling | n.t.b. |

### 8.2 Prijsregels
- **Fundament is verplicht vóór een sprint**, tenzij de scan aantoont dat de basis al op orde is. Dat is geen verkooptruc maar een leveringsvoorwaarde: zonder laag 0 en 1 is de sprint niet houdbaar. Zet dit letterlijk zo in de offerte — het maakt de USP tastbaar en voorkomt discussie achteraf.
- Fundament en sprint samen als **AI-Fundament + Eerste Toolkit** aanbieden voor €5.500 – €8.500. Dat is het standaard-startpakket en de meest verkochte regel.
- Scanbedrag wordt verrekend bij doorgang naar een sprint binnen 30 dagen. Dat maakt de instap risicoloos en dwingt tempo af.
- Betaling: 50% vooraf, 50% bij oplevering. Retainer maandelijks vooraf.
- Geldigheid offerte: 14 dagen.
- Nooit uurtarief noemen. Alles per fase met vaste scope.
- Meerwerk in blokken van €450 (halve dag).
- Geen korting; wél scope verkleinen — dit geldt ook voor de retainer: nooit korting op een trede, wél afschalen naar een lagere trede (zie 8.5).

### 8.3 Onderbouwing
Een medewerker van €45k kost het bedrijf circa €65k per jaar. Vier uur tijdwinst per week bij drie medewerkers is ruwweg €25.000 per jaar. Een sprint van €3.500 verdient zich dan binnen twee maanden terug. **Dat sommetje staat in elke offerte, ingevuld met hun eigen cijfers.**

### 8.4 Weg naar €10.000 in 3 maanden

| Bron | Aantal | Bedrag | Totaal |
|---|---|---|---|
| AI Readiness Scan | 4 | €750 | €3.000 |
| Toolkit Sprint | 1 | €3.500 | €3.500 |
| In-company workshop | 2 | €950 | €1.900 |
| Retainer (2 klanten × 2 mnd) | 4 mnd | €750 | €3.000 |
| **Totaal** | | | **€11.400** |

Benodigde funnel: circa 60 gekwalificeerde contacten → 20 gesprekken → 8 voorstellen → 5 opdrachten. Dat is de sturingsnorm voor de acquisitie.

### 8.5 Retainer-afbouwladder (anti-churn)

**Probleem dat dit oplost:** SWOT-bedreiging 6 — klant heeft na het fundament/sprint zijn AI-gebruik op orde, voelt geen actieve waarde meer maandelijks, en zegt de volledige retainer op. Weg is de terugkerende omzet én het onderhoudscontact.

**Principe:** in plaats van een aan/uit-retainer, vier tredes die in prijs en dienstverlening afbouwen. Bij dreigende opzegging wordt nooit "opzeggen of niets" aangeboden, maar altijd eerst een trede lager. Onderin zit een bodemtrede die zo laag geprijsd is dat de klant er nooit meer bewust over nadenkt — en die desondanks ruim boven Ricks eigen kostprijs (grotendeels geautomatiseerde monitoring, nauwelijks actieve tijd) blijft liggen. Zo loopt de retainer jarenlang door zonder gesprek, terwijl de waarde (werkende koppelingen, geen stille storingen) de prijs ruim overtreft.

| Trede | Naam | Prijs p/m | Inhoud | Voor wie |
|---|---|---|---|---|
| 1 | **AI-Partner Groei** | €1.250 – €2.000 | nieuwe skills en koppelingen, actieve doorontwikkeling, helpdesk binnen 1 werkdag, kwartaalworkshop | klant breidt AI-gebruik nog actief uit |
| 2 | **AI-Partner Onderhoud** | €750 – €950 | onderhoud bestaande skills/koppelingen, helpdesk binnen 2 werkdagen, kwartaalupdate, kleine aanpassingen | gebruik is stabiel, weinig nieuwbouw nodig |
| 3 | **AI-Basis** | €350 – €450 | maandelijkse health-check van koppelingen en kennisbestanden, mailsupport, 1 kleine aanpassing per kwartaal | klant redt zich grotendeels zelf |
| 4 | **AI-Vangnet** | €99 – €149 | geautomatiseerde monitoring van MCP-/n8n-koppelingen en kennisbestanden, noodfix binnen 5 werkdagen bij storing, geen actief contact tenzij er iets stukgaat | klant wil (bijna) stoppen |

**Waarom trede 4 werkt als bodem:**
- Kostprijs voor Rick is bijna nul: monitoring loopt via hetzelfde geautomatiseerde dashboard voor alle vangnet-klanten samen, geen losse arbeidstijd per klant tenzij er een storing is.
- Waarde voor de klant blijft hoog: koppelingen breken vaak stil (API-wijziging bij de softwareleverancier, aflopend token, gewijzigd model) zonder dat iemand het merkt tot er al weken foute output is gebruikt. €99–149/mnd tegen dat risico is voor een MKB-directie geen bedrag om over te bellen.
- Vergelijkbaar met een streamingabonnement: te klein om over na te denken, te vervelend om op te zeggen voor het bedrag dat het scheelt.

**Regel voor het gesprek — nooit proactief afschalen aanbieden.** Trede-verlaging wordt alleen ter sprake gebracht wanneer:
1. de klant zelf aangeeft te willen stoppen of te bezuinigen, of
2. gebruiksdata (skill-gebruik, supportvragen) over twee opeenvolgende kwartalen structureel onder de drempel van de huidige trede zakt.

Bij zo'n moment is de zin altijd: *"Voordat we het helemaal stopzetten — we kunnen ook terug naar [trede], dat kost bijna niks, maar je koppelingen en kennisbestanden blijven wel gecontroleerd draaien. Zullen we dat doen in plaats van volledig stoppen?"* Nooit zelf het opzeggen voorstellen als eerste optie.

**Reactivatie:** vanuit trede 3 of 4 is opschalen laagdrempelig — geen nieuw traject, gewoon een trede omhoog, ingaand volgende factuurmaand. Dit is het natuurlijke instappunt zodra een klant weer gaat groeien of een nieuwe afdeling erbij pakt.

**Verwerking in KPI's:** retentie meten op twee niveaus — "retainer actief (ongeacht trede)" en "retainer op trede 1–2 (hoogwaardig)". Trede 4-klanten tellen mee voor omzetbehoud, niet voor groei.

---

## 9. SWOT

### Sterktes
1. Bouwt en levert zelf, geen doorverkoop
2. Ontwerp- en communicatievaardigheid maakt output begrijpelijk voor niet-technische klanten
3. Bestaande MKB-klantenkring en regionaal netwerk voor de eerste opdrachten
4. Snel: van scan naar werkende oplevering in weken, niet kwartalen
5. Lage vaste kosten, dus scherpe prijs zonder margeverlies

### Zwaktes
1. Solo-operator: capaciteitsplafond en leveringsrisico bij ziekte
2. Nog geen referenties of casussen in deze specifieke lijn
3. Geen merkgezag als "AI-partij" — bekend als designer
4. Geen certificering, geen securitydossier voor kritische klanten
5. Aandacht verdeeld over design/web en deze nieuwe lijn

### Kansen
1. **Softwareleveranciers bouwen AI standaard in hun pakketten in.** Dit is geen bedreiging maar de motor onder de vraag: elke ondernemer zet die knoppen aan, ziet dat het weinig oplevert, en gaat zoeken naar het waarom. Dat waarom is de structuur eronder — precies het aanbod. Elke nieuwe AI-functie die een leverancier uitrolt, is gratis vraagcreatie en levert een prospect op die de teleurstelling al zelf heeft gevoeld.
2. Regio Brainport: technisch bewustzijn hoog, uitvoering laag
3. Grote adviesbureaus richten zich op corporates; 10–25 fte is onderbediend
4. Personeelskrapte maakt tijdwinst direct waardevol
5. Subsidies voor scholing/innovatie (o.a. SLIM) verlagen de drempel
6. Doorverwijzing via boekhouders, IT-partners en brancheverenigingen
7. Toolkits en fundamentsjablonen per branche zijn later te productiseren en te licentiëren
8. Fundamentwerk is model- en toolonafhankelijk en veroudert dus nauwelijks
9. **Lokale AI als latere add-on** opent zorg, accountancy en advocatuur, en is het antwoord op elke AVG- en AI Act-bezwaar. Nog niet rijp, wel de logische volgende trede op het fundament

### Bedreigingen
1. **Ondernemers denken dat de ingebouwde AI-knoppen genoeg zijn** en voelen geen urgentie tot ze er zelf op stukgelopen zijn. Dit is de echte bedreiging, niet de knoppen zelf.
2. "Structuur op orde brengen" klinkt als saai, duur en vaag. Verkooprisico: het moet in resultaten verteld worden, nooit in het woord *structuur*.
3. Prijsdruk door AI-consultants zonder uitvoeringskracht
4. Snel veranderend landschap maakt toolkits (laag 2 en 3) verouderd
5. AVG/AI Act-eisen verzwaren richting zakelijke en zorgklanten
6. ~~Klanten die na het fundament zelf verdergaan en de retainer laten vallen~~ — grotendeels ondervangen door de retainer-afbouwladder (8.5): klant valt niet meer op nul, maar zakt naar een bodemtrede die blijft lopen

### Strategische conclusies
- **S×O1:** de teleurstelling over ingebouwde AI-knoppen is de scherpste haak in alle content, outreach en het webinar. Openingszin: "Jullie hebben de AI-functies aangezet en er gebeurde weinig. Dat ligt niet aan de AI."
- **T1×T2:** nooit "structuur" of "organisatie-inrichting" verkopen. Verkoop het als *"AI die eindelijk wél weet waar alles staat"* en toon vóór/ná met dezelfde knop in hun eigen software.
- **S×O:** eerste twee fundamenten tegen instapprijs bij bestaande klanten, uitsluitend om casussen te maken.
- **W×T4:** onderhoud en actualiteit inbouwen in de retainer, uitgewerkt als afbouwladder (8.5) zodat de retainer nooit in één keer naar nul valt.
- **W1:** vanaf klant 5 een vaste freelance-uitvoerder aanhaken voor bouwwerk.

---

## 10. Marketingstrategie

### 10.1 Positioneringskeuze
Niche op **bedrijfsgrootte en regio**, niet op techniek. Elke uiting begint bij hun probleem, nooit bij het model of de tool.

### 10.2 Kanaalprioriteit

| Prio | Kanaal | Doel | Ritme |
|---|---|---|---|
| 1 | LinkedIn (persoonlijk profiel Rick) | autoriteit + inbound | 3 posts/week |
| 2 | Webinar (maandelijks, gratis, 60 min) | lead-engine | 1 per maand |
| 3 | Directe outreach naar shortlist | opdrachten nu | 20 per week |
| 4 | Partnerkanaal (boekhouders, IT-partners, brancheverenigingen) | doorverwijzing | 2 gesprekken/week |
| 5 | Website + landingspagina's per branche | conversie + SEO | doorlopend |
| 6 | Nieuwsbrief | nurturing | 2× per maand |
| 7 | Offline: ondernemersavonden, netwerkclubs | vertrouwen | 1× per maand |

Geen betaalde advertenties in de eerste 3 maanden. Eerst boodschap valideren via organische kanalen en gesprekken.

### 10.3 Contentpijlers (LinkedIn + nieuwsbrief)
1. **Laten zien** — korte demo van één skill, met resultaat ("offerte in 4 minuten in plaats van 40")
2. **Ontnuchteren** — wat AI in het MKB níet doet, mislukte pilots, waarom tools blijven liggen
3. **Uitleggen** — skills, MD-bestanden, MCP, toolkits, in mensentaal
4. **Bewijzen** — casussen, cijfers, klantcitaten
5. **Meekijken** — bouwen in de openbaarheid, eigen werkwijze delen

Vaste haak in de eerste 3 woorden. Elke post eindigt in een concrete vervolgstap (webinar, scan, gesprek).

### 10.4 Webinar als motor
Vast format, maandelijks herhaald, één onderwerp:
**"Jullie hebben de AI-knoppen aangezet. Waarom er niks gebeurt."**

Opbouw: 5 min probleemherkenning (iedereen heeft die knoppen al aan) → 15 min waarom het misgaat: het lagenmodel, laag 0 en 1 ontbreken → 25 min live demo, dezelfde AI-functie vóór en ná een opgeruimd fundament → 10 min routekaart → 10 min vragen → aanbod: gratis intake of scan tegen actieprijs.

Deze titel is scherper dan een neutrale "waar begin je"-titel omdat hij een teleurstelling benoemt die de doelgroep al heeft gevoeld. Alternatieve titel voor koudere lijsten: "AI invoeren met 10–25 medewerkers: waar begin je?"
Doel per editie: 25 aanmeldingen, 12 aanwezigen, 4 intakes, 1–2 scans.
Opname wordt hergebruikt als contentbron en als leadmagneet.

### 10.5 Leadmagneten
1. **AI-Startgids voor MKB (10–25 medewerkers)** — pdf, 12 pagina's, de routekaart
2. **AI-Readiness checklist** — 20 vragen, zelfscore
3. **Gratis proef-toolkit** — 3 werkende skills, direct bruikbaar, met PRJCT-signatuur
4. **Tijdwinst-calculator** — invullen, uitkomst in uren en euro's per jaar

### 10.6 Salesflow
Webinar of outreach → intake 30 min (video) → scanvoorstel → scan uitvoeren → presentatie roadmap → sprintvoorstel (verrekening scan) → sprint → 30-dagen-check → retainervoorstel (starten op trede 1 of 2, zie 8.5).

Vaste opvolging: dag 1 samenvatting, dag 3 casus, dag 7 telefoon, dag 14 laatste voorstel, dag 45 heropening.

### 10.7 90-dagenplan

**Maand 1 — fundament en eerste bewijs**
Positionering en prijskaart vastzetten · landingspagina live · LinkedIn-profiel herschrijven · 15 doelgroepgesprekken · 2 leadmagneten af · eerste webinar plannen · eerste scan verkopen aan bestaande klant

**Maand 2 — motor aanzetten**
Eerste webinar draaien · 3 scans uitvoeren · eerste sprint verkopen en starten · casus #1 documenteren · 3 partnergesprekken · outreach op 20 contacten per week

**Maand 3 — herhalen en borgen**
Tweede webinar · sprint opleveren en meten · retainer aanbieden · casus #2 · branchelandingspagina's live · besluit over het eerste branchepakket

### 10.8 KPI's

| KPI | Norm maand 3 |
|---|---|
| Gekwalificeerde contacten per maand | 20 |
| Intakegesprekken per maand | 8 |
| Scanverkoop per maand | 2 |
| Scan → sprint conversie | ≥ 50% |
| Webinaraanmeldingen per editie | 25 |
| Omzet uit deze lijn per maand | €3.500 |
| LinkedIn-volgers uit doelgroep | +400 |

---

## 11. Uitvoeringsarchitectuur (basis voor agents en delegatie)

Elk blok hieronder wordt later een eigen agent of skill met eigen bestanden en eigen output.

| # | Module | Verantwoordelijkheid | Belangrijkste output |
|---|---|---|---|
| 1 | **Sales-agent** | prospectlijst, kwalificatie, outreach, opvolging | leadlijst, pitchscripts, opvolgstatus |
| 2 | **Scan-agent** | intakeverwerking, procesinventarisatie, use-case-prioritering | `[Klant]_Scan_[datum].pdf`, roadmap, businesscase |
| 2b | **Fundament-agent** | domeinindeling, procesbeschrijvingen, eigenaarschapsmatrix, mappen- en naamgevingsstructuur, bronwaarheid, MD-kennisbasis per domein | `[Klant]_Fundament_[datum]/` met structuurplan en kennisbestanden |
| 3 | **Toolkit-builder-agent** | skills, MD-kennisbasis, plugins, documentatie | toolkitmap per klant |
| 4 | **Integratie-agent** | MCP-koppelingen en n8n-workflows | node-voor-node bouwbeschrijving, werkende koppeling |
| 5 | **Training-agent** | trainingsopzet, naslag, webinarmateriaal | draaiboek, slides, hand-out |
| 6 | **Content-agent** | LinkedIn, nieuwsbrief, landingspagina's | contentkalender, teksten |
| 7 | **Offerte-agent** | voorstellen op vaste prijskaart | `[Klant]_Offerte_[datum].pdf` |
| 8 | **Rapportage-agent** | 30/60-dagen-metingen, casussen, KPI-dashboard | resultatenoverzicht, casus |
| 9 | **Retainer-agent** *(nieuw)* | trede-toewijzing, gebruiksmonitoring per klant, afschaal-/opschaalgesprekken op basis van 8.5 | tredestatus per klant, signalenlijst voor afschaalgesprek |

**Gedeelde basisbestanden (eerst bouwen, alle agents lezen ze):**
`prijskaart.md` · `personas.md` · `positionering.md` · `usps.md` · `bezwaren-en-antwoorden.md` · `klantdossier-template.md` · `toolkit-standaard.md` · `retainer-tredes.md`

**Naamgeving:** `[Klant]_[Type]_[Datum]` · nieuwe varianten altijd apart opslaan, nooit overschrijven.

---

## 12. Openstaande beslissingen

1. Merknaam: PRJCT AI als lijn, of een eigen merk los van PRJCT Agency?
2. Eerste branche om in te dominéren: zakelijke dienstverlening of installatie/techniek? (advies: zakelijke dienstverlening, hoogste tekstvolume en snelste bewijs)
3. Welke twee bestaande klanten worden de casusklanten tegen instapprijs?
4. Webinar: eigen platform of via een partner met bestaand publiek?
5. Wordt de proef-toolkit publiek weggegeven, en zo ja welke drie skills?
6. Marktcijfers uit 2.4 hard maken met KvK/Company.info-data.
7. Lokale AI (1.5): wanneer wordt de eigen proefopstelling ingepland, en op welke hardware? Pas daarna een aanbod formuleren. Tot die tijd alleen benoemen als richting, nooit als dienst.
8. Naamgeving van het kernproduct: "Bedrijfsfundament", "AI-Fundament" of "AI-Ready Bedrijf"? De naam moet resultaat suggereren, niet structuurwerk — dat laatste klinkt als saai en duur.
9. Hoe wordt de vangnet-monitoring (trede 4, 8.5) technisch gebouwd — losse n8n-workflow per klant of één gedeeld monitoring-dashboard over alle vangnet-klanten? Bepaalt de echte kostprijs van de bodemtrede.

---

*Volgende stap: hoofdstuk voor hoofdstuk uitwerken tot werkdocumenten, te beginnen bij prijskaart, personas en bezwaren-en-antwoorden — die drie voeden elke agent.*
