# Structuurplan — [Klant] [MOCK]

**Datum:** [datum] · **Interne eigenaar bij klant:** [naam]

## 1. Domeinen

| Domein | Eigenaar | Kernprocessen | Systemen |
|---|---|---|---|
| Sales | | | |
| Operations | | | |
| Marketing | | | |
| Finance | | | |
| HR | | | |

## 2. Bronwaarheid per kerngegeven

| Gegeven | De waarheid staat in | Niet in | Eigenaar |
|---|---|---|---|
| Klantgegevens | | | |
| Prijzen en tarieven | | | |
| Offertes | | | |
| Projectstatus | | | |
| Personeelsgegevens | | | |

## 3. Mappenstructuur

```
[Bedrijf]/
├── 01_klanten/
│   └── [Klantnaam]/
│       ├── 01_offertes/
│       ├── 02_uitvoering/
│       └── 03_facturen/
├── 02_intern/
├── 03_bedrijfskennis/
└── 99_archief/
```

Maximaal drie niveaus diep.

## 4. Naamgeving

1. `[Klant]_[Type]_[JJJJ-MM-DD]`
2. Datums altijd JJJJ-MM-DD
3. Geen spaties, gebruik `_`
4. Varianten met `_v2`, nooit overschrijven
5. Verouderd naar `99_archief/`, niet verwijderen

## 5. Wat er verandert voor wie

| Wie | Wat verandert | Wat blijft |
|---|---|---|
| | | |

## 6. Migratieplan

| Stap | Wat | Wanneer | Wie |
|---|---|---|---|
| 1 | Back-up | | |
| 2 | | | |
