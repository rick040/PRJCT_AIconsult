# Fundamentsjabloon — zakelijke dienstverlening [MOCK]

Startpunt voor accountants, adviesbureaus, makelaars, HR en recruitment. Aanpassen per klant, nooit één op één overnemen.

## Domeinen

| Domein | Kernprocessen | Typische systemen |
|---|---|---|
| Sales | offerte, opvolging, contract | CRM, mail |
| Dossier/uitvoering | dossieropbouw, verslaglegging, oplevering | vakpakket, Drive/SharePoint |
| Finance | facturatie, urenregistratie, debiteuren | boekhoudpakket |
| Marketing | website, nieuwsbrief, sociale kanalen | |
| HR | werving, verzuim, gesprekken | |

## Bronwaarheid, typische valkuilen
| Gegeven | Waar het hoort | Waar het meestal ook staat |
|---|---|---|
| Klantgegevens | CRM | mailbox van de accountmanager |
| Tarieven | prijslijst | laatste offerte |
| Dossierstatus | vakpakket | hoofd van de behandelaar |

## Mappenstructuur
```
[Bedrijf]/
├── 01_klanten/[Klant]/{01_offertes,02_dossier,03_facturen}
├── 02_intern/
├── 03_bedrijfskennis/
└── 99_archief/
```

## Aandachtspunt
Deze branche heeft vaak beroepsgeheim of tuchtrecht. Spelregels-AI eerst, koppelingen daarna.
