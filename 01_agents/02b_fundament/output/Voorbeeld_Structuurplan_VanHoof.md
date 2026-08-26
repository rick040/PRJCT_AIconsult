# Structuurplan — Van Hoof Installaties [MOCK, voorbeelduitvoer]

**Datum:** 2026-10-05 · **Interne eigenaar bij klant:** Wendy Smulders (planner)

> Voorbeelduitvoer van de fundament-agent, gebaseerd op het scanrapport van 2026-09-16. Geen echt klantdossier.

## 1. Domeinen

Vier scherpe domeinen, geen zes vage. Marketing en HR zijn bij Van Hoof geen aparte functie, dus niet apart opgenomen.

| Domein | Eigenaar | Kernprocessen | Systemen |
|---|---|---|---|
| Sales | Bas van Hoof | Offerteaanvraag verwerken, offerte opstellen, opvolgen, order vastleggen | Outlook, Word, website-contactformulier |
| Operations | Wendy Smulders | Planning inplannen, werkbon uitwerken, materiaal bestellen | Outlook-agenda, papieren werkbon (foto via WhatsApp) |
| Finance | Bas van Hoof (extern: boekhouder) | Factureren, inkoopfacturen verwerken | Boekhoudpakket (extern beheerd) |
| Directie | Bas van Hoof | Jaarplanning, personeel, grote inkoop | — |

## 2. Bronwaarheid per kerngegeven

| Gegeven | De waarheid staat in | Niet in | Eigenaar |
|---|---|---|---|
| Klantgegevens | Nieuw: `02_klanten/[klantnaam]/` map per klant | Niet meer los in mail | Wendy |
| Prijzen en tarieven | Nieuw: `03_bedrijfskennis/diensten-en-prijzen.md` | Niet meer in Bas' hoofd of het Excel-bestand uit 2023 | Bas |
| Offertes | `02_klanten/[klantnaam]/01_offertes/` | Niet meer los in de mailbox | Bas |
| Projectstatus | Wendy's planningsoverzicht (nieuw, één bestand) | Niet meer los bij Bas en Wendy apart | Wendy |
| Personeelsgegevens | Boekhoudpakket / extern administratiekantoor | — | Bas |

## 3. Mappenstructuur

```
VanHoof-AI/
├── 01_klanten/
│   └── [Klantnaam]/
│       ├── 01_offertes/
│       ├── 02_uitvoering/
│       └── 03_facturen/
├── 02_intern/
├── 03_bedrijfskennis/
└── 99_archief/
```

Maximaal drie niveaus diep, zoals voorgeschreven in `toolkit-standaard.md`.

## 4. Naamgeving

1. `[Klant]_[Type]_[JJJJ-MM-DD]`
2. Datums altijd JJJJ-MM-DD
3. Geen spaties, gebruik `_`
4. Varianten met `_v2`, nooit overschrijven
5. Verouderd naar `99_archief/`, niet verwijderen

## 5. Wat er verandert voor wie

| Wie | Wat verandert | Wat blijft |
|---|---|---|
| Bas | Prijzen komen uit één bestand, niet meer uit het hoofd | Hij blijft zelf offertes beoordelen en tekenen |
| Wendy | Krijgt eigenaarschap over klantmappen en planning, wordt beheerder van de toolkit | Planning blijft in de agenda, alleen nu gekoppeld aan vaste mappen |
| Personeel op de vloer | Werkbon straks digitaal in plaats van foto via WhatsApp (fase 2) | Werkbon blijft hetzelfde papieren formulier tot fase 2 |

## 6. Migratieplan

| Stap | Wat | Wanneer | Wie |
|---|---|---|---|
| 1 | Back-up van bestaande mailbox-bijlagen en het Excel-prijsbestand | week 1 | Rick |
| 2 | Bestaande offertes (lopend jaar) overzetten naar nieuwe klantmappen | week 1-2 | Rick, met Wendy |
| 3 | Prijslijst controleren en vastleggen in `diensten-en-prijzen.md` | week 2 | Bas |
| 4 | Oud materiaal naar `99_archief/`, niets verwijderd | week 2 | Rick |
| 5 | Overdracht aan Wendy, uitleg waarom de indeling zo is gekozen | week 3 | Rick, Wendy, Bas |
