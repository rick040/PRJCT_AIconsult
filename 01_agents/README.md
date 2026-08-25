# Agents

Elke map is één agent met één verantwoordelijkheid. De indeling volgt de klantreis:

| # | Map | Fase in de klantreis |
|---|---|---|
| 1 | `01_sales` | Lead vinden en kwalificeren |
| 2 | `02_scan` | Diagnose stellen |
| 2b | `02b_fundament` | Laag 0 en 1 neerzetten |
| 3 | `03_toolkit-builder` | Laag 2 bouwen |
| 4 | `04_integratie` | Laag 3 bouwen |
| 5 | `05_training` | Laag 4 overdragen |
| 6 | `06_content` | Doorlopend, vult de funnel |
| 7 | `07_offerte` | Doorlopend, na elke fase |
| 8 | `08_rapportage` | Meten, casus maken, retainer verkopen |

## Vaste indeling per agentmap

```
[agent]/
├── AGENT.md      # rol, input, output, werkwijze, kwaliteitseisen
├── templates/    # vaste sjablonen die deze agent invult
└── output/       # generiek werk, niet klantgebonden
```

Klantgebonden output gaat nooit hierheen maar naar `02_klanten/[Klant]/`.

## Elke AGENT.md heeft dezelfde kop

Rol · Leest altijd · Input · Output · Werkwijze · Kwaliteitseisen · Nooit
