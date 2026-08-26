# AI Readiness Scan — Van Hoof Installaties [MOCK, voorbeelduitvoer]

**Datum:** 2026-09-16 · **Uitgevoerd door:** Rick van Mierlo · **Contactpersoon:** Bas van Hoof, DGA

> Dit is een voorbeelduitvoer van de scan-agent, geen echt klantrapport. Bedoeld om het rapportformat en de redeneerstappen te tonen. Cijfers zijn illustratief, niet gevalideerd bij een echte klant.

## Samenvatting

Van Hoof Installaties draait op 18 man en een DGA die zelf 's avonds offertes uittypt. De grootste winst zit in laag 0: offertes staan half in de mail, half in een Wordmap, prijzen kloppen daardoor niet altijd. Eerste stap: Bedrijfsfundament, daarna een Toolkit Sprint voor sales.

## 1. Nulmeting

| Vraag | Antwoord |
|---|---|
| Welke AI-functies staan aan | Copilot in Outlook (standaard aan via Microsoft 365), niemand gebruikt het actief |
| Wat leverde dat op | Concepttekst voor mails, wordt zelden gebruikt omdat toon niet klopt |
| Grootste tijdvreter | Offertes opstellen en opvolgen |
| Uren per week | Circa 6 uur, verdeeld over Bas en planner Wendy |
| Kosten per jaar | Circa €19.500 (op basis van geschatte belaste kosten, in een echt traject met hun loonkosten) |

## 2. Waar het nu op vastloopt

Offerteaanvragen komen binnen via mail, telefoon en het contactformulier op de site. Bas zet ze zelf om in een offerte in Word, aan de hand van een prijslijst die deels in zijn hoofd zit en deels in een oud Excel-bestand van 2023. Planner Wendy weet niet altijd of een offerte al verstuurd is, omdat de status nergens gezamenlijk staat. Copilot in Outlook kan hierbij niet helpen: het model heeft geen toegang tot de actuele prijslijst en weet niet welke offertes al liepen. Dit is precies het patroon uit `lagenmodel.md`: een AI-knop die aanstaat, boven een laag 0 die niet klopt.

## 3. Laagstatus

| Laag | Status | Wat we zagen | Wat er moet gebeuren |
|---|---|---|---|
| 0. Structuur | rood | Offertes deels in mail, deels in Word, geen vaste mappen, prijslijst verouderd | Domeinindeling, mappenstructuur, één bronwaarheid voor prijzen |
| 1. Context | rood | Geen vastgelegde tone of voice, procedures zitten in Bas' hoofd | Kennisbestanden bedrijf, diensten en prijzen, procedures |
| 2. Werkinstructies | rood | Niemand heeft een vaste manier van offertes opstellen | Skill sales-offerte-opstellen, na het fundament |
| 3. Koppelingen | rood | Contactformulier site niet gekoppeld aan iets, alles handmatig overgetypt | n8n-koppeling mail/formulier naar offerteproces, na de toolkit |
| 4. Borging | rood | Niemand behalve Bas kan een offerte opstellen | Training en champion, Wendy is kandidaat |

## 4. Vijf use-cases, geprioriteerd

| # | Use-case | Domein | Tijdwinst p/w | Haalbaarheid | Laag |
|---|---|---|---|---|---|
| 1 | Offerte opstellen vanuit aanvraag | Sales | 4 uur | Hoog | 2 |
| 2 | Werkbon uitwerken naar factuurregels | Operations | 2 uur | Hoog | 2 |
| 3 | Mailtriage offerteaanvragen | Sales | 1,5 uur | Middel | 3 |
| 4 | Planning-overzicht bijhouden | Operations | 1 uur | Middel | 2 |
| 5 | Nazorgmail na oplevering | Sales | 0,5 uur | Hoog | 2 |

## 5. Businesscase

| Post | Bedrag |
|---|---|
| Tijdwinst per week | 6 uur (use-case 1 en 2) |
| Betrokken medewerkers | Bas (DGA) en Wendy (planner) |
| Kosten per uur | circa €65 (DGA) en €35 (planner), in een echt traject hun eigen loonkosten |
| Besparing per jaar | circa €15.600 |
| Investering eerste fase | €5.500 tot €8.500 (Startpakket: Fundament + Eerste Toolkit) |
| Terugverdientijd | circa 4 tot 6 maanden |

## 6. Roadmap

| Fase | Wat | Wanneer | Investering |
|---|---|---|---|
| 1 | Bedrijfsfundament | week 1 tot 4 | €2.500 tot €5.000 |
| 2 | Toolkit Sprint Sales | week 5 tot 8 | €2.500 tot €4.500 |
| 3 | Koppeling contactformulier en mail (n8n) | later, na toolkit | €750 tot €2.500 |

## 7. Eerste stap

Startpakket Fundament + Eerste Toolkit, €5.500 tot €8.500, doorlooptijd 6 tot 8 weken. Scanbedrag van €750 wordt verrekend bij doorgang binnen 30 dagen. Van Hoof levert: toegang tot de mailbox en de huidige prijslijst, en een dagdeel van Bas en Wendy samen in week 1.
