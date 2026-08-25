# Klanten

Eén map per klant. Kopieer `_TEMPLATE/` en hernoem naar de bedrijfsnaam zonder spaties.

```
02_klanten/
├── _TEMPLATE/          # niet in gebruik nemen, alleen kopiëren
└── [Klantnaam]/
    ├── klantdossier.md # eerst invullen, elke agent leest dit
    ├── 01_intake/
    ├── 02_scan/
    ├── 03_fundament/
    ├── 04_toolkit/
    └── 05_rapportage/
```

## Regels

- `klantdossier.md` wordt als eerste ingevuld en bij elke fase bijgewerkt
- Naamgeving van bestanden: `[Klant]_[Type]_[JJJJ-MM-DD].[ext]`
- Nooit overschrijven. Varianten krijgen `_v2`, `_v3`
- Klantdata blijft in deze map. Nooit kopiëren naar `01_agents/`, `04_bibliotheek/` of content
- Afgeronde klanten blijven staan. Verouderd materiaal binnen de klantmap naar een eigen `99_archief/`
