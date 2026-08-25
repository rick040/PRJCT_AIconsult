# Toolkit-standaard

> Hoe elke klanttoolkit eruitziet. De toolkit-builder-agent volgt dit exact.
> Laatst bijgewerkt: 2026-08-25 · v1.0

## Doel

Een toolkit is overdraagbaar, begrijpelijk voor een niet-technische medewerker, en blijft werken zonder PRJCT AI. Als een toolkit alleen bij ons werkt, is hij niet af.

## Vaste mapstructuur bij de klant

```
[Bedrijfsnaam]-AI/
├── LEESMIJ.md                  # één A4: wat is dit, hoe begin ik, wie beheert het
├── 00_bedrijf/                 # laag 1: context
│   ├── bedrijf.md              # wat we doen, voor wie, hoe we praten
│   ├── diensten-en-prijzen.md
│   ├── klanten-en-doelgroep.md
│   ├── procedures.md
│   └── spelregels-ai.md        # governance: wat mag er wel en niet in
├── 01_skills/                  # laag 2: werkinstructies
│   ├── [domein]-[taak].md
│   └── ...
├── 02_koppelingen/             # laag 3
│   ├── mcp-overzicht.md
│   └── n8n-workflows.md
├── 03_training/                # laag 4
│   ├── naslag.md
│   └── opnames.md
└── 04_onderhoud/
    ├── changelog.md
    └── openstaand.md
```

## Standaard voor een skill

Elke skill is één bestand en bevat, in deze volgorde:

1. **Titel en één zin** wat de skill doet
2. **Wanneer gebruiken** en wanneer niet
3. **Wat je nodig hebt** aan input
4. **Stappen** die het model volgt
5. **Vorm van de uitkomst** met een voorbeeld
6. **Wat er mis kan gaan** en wat de gebruiker dan doet
7. **Eigenaar en laatst bijgewerkt**

Zie `04_bibliotheek/skills/_SKILL-TEMPLATE.md`.

## Kwaliteitseisen bij oplevering

- [ ] Elke skill is minimaal drie keer getest op echte data van de klant
- [ ] Elke skill benoemt wat er mis kan gaan
- [ ] LEESMIJ past op één A4
- [ ] Er is één interne eigenaar aangewezen, met naam
- [ ] Governance-A4 is besproken en akkoord
- [ ] Niets in de toolkit verwijst naar een tool die alleen Rick heeft
- [ ] Nulmeting en 30-dagenmeting zijn ingepland

## Naamgeving

Skills: `[domein]-[taak].md`, bijvoorbeeld `sales-offerte-opstellen.md`, `operations-werkbon-uitwerken.md`.
Domeinen: sales, operations, marketing, finance, hr, directie.
