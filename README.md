# PRJCT AI

Werkrepo van de AI-implementatielijn van PRJCT Agency. Rick van Mierlo, Eindhoven/Geldrop.

**Doelgroep:** MKB-bedrijven met 10 tot 25 medewerkers in de Brainport-regio die AI willen invoeren maar niet weten waar te beginnen.

**Kernbelofte:** AI werkt pas als je bedrijf erop is gebouwd. Wij zetten eerst de structuur neer en bouwen daar de AI-werkplek bovenop.

> Deze repo is tegelijk het product. De indeling hier is dezelfde die we bij klanten neerzetten. Als het hier rommelig wordt, verkopen we iets wat we zelf niet doen.

## Structuur

```
.
├── CLAUDE.md              # werkinstructie, wordt door elke agent gelezen
├── 00_kern/               # bron van waarheid, alle agents lezen dit
├── 01_agents/             # negen agents, één map per verantwoordelijkheid
├── 02_klanten/            # één map per klant, kopie van _TEMPLATE
├── 03_producten/          # productdefinities
├── 04_bibliotheek/        # herbruikbaar materiaal, zonder klantdata
├── 05_bedrijf/            # bedrijfsvoering PRJCT AI zelf
└── 99_archief/            # verouderd, niets wordt verwijderd
```

## 00_kern: begin hier

Deze tien bestanden bepalen alles wat er verder gebeurt. Verander je hier iets, dan verandert het overal.

| Bestand | Waarvoor |
|---|---|
| `positionering.md` | wie we zijn, wat we wel en niet doen |
| `lagenmodel.md` | de inhoudelijke kern van de aanpak |
| `prijskaart.md` | elke prijsuitspraak komt hier vandaan |
| `personas.md` | Bas, Marloes, Joris |
| `usps.md` | wat ons onderscheidt, op volgorde |
| `bezwaren-en-antwoorden.md` | twaalf bezwaren met vaste antwoorden |
| `tone-of-voice.md` | hoe we schrijven |
| `doelgroep.md` | wie we bedienen en wie niet |
| `klantdossier-template.md` | het dossier per klant |
| `toolkit-standaard.md` | hoe elke klanttoolkit eruitziet |

## 01_agents: de negen agents

| # | Agent | Verantwoordelijkheid | Output |
|---|---|---|---|
| 1 | Sales | Prospectlijst, kwalificatie, outreach, opvolging | Leadlijst, pitchscripts, opvolgstatus |
| 2 | Scan | Intakeverwerking, procesinventarisatie, use-case-prioritering | Scanrapport, roadmap, businesscase |
| 2b | Fundament | Domeinindeling, processen, eigenaarschap, mappen, bronwaarheid, kennisbasis | Structuurplan en kennisbestanden per klant |
| 3 | Toolkit-builder | Skills, plugins, documentatie | Toolkitmap per klant |
| 4 | Integratie | MCP-koppelingen en n8n-workflows | Bouwbeschrijving, werkende koppeling |
| 5 | Training | Trainingsopzet, naslag, webinarmateriaal | Draaiboek, slides, hand-out |
| 6 | Content | LinkedIn, nieuwsbrief, landingspagina's | Contentkalender, teksten |
| 7 | Offerte | Voorstellen op de vaste prijskaart | Offerte per klant |
| 8 | Rapportage | 30/60-dagenmetingen, casussen, KPI's | Resultatenoverzicht, casus |

Elke agentmap bevat `AGENT.md` (rol, input, output, werkwijze, kwaliteitseisen, wat hij nooit doet), een `templates/` map en een `output/` map.

## Werkregels

1. Klantdata blijft in `02_klanten/`. Nooit kopiëren naar agents, bibliotheek of content.
2. Naamgeving: `[Klant]_[Type]_[JJJJ-MM-DD].[ext]`
3. Nooit overschrijven. Varianten krijgen `_v2`, `_v3`.
4. Verouderd materiaal gaat naar `99_archief/`, wordt niet verwijderd.
5. Nooit een prijs of belofte gebruiken die niet in `00_kern/` staat.
6. Wijzigingen in `00_kern/` alleen met akkoord van Rick.

## Status

Fase: opbouw. Bestanden met `[MOCK]` in de titel of `[TE BEPALEN: ...]` in de tekst zijn skeletten en voorbeelden. Vervangen zodra er echt materiaal is. Nooit als feit richting een klant gebruiken.

## Waar je begint als je vandaag gaat werken

1. `05_bedrijf/roadmap/dag-1.md` als je nog moet starten. Zeven taken, ongeveer vijf uur
2. `05_bedrijf/roadmap/routekaart.md` voor de volgorde daarna: zes blokken van idee naar draaiende praktijk
3. `05_bedrijf/framework/basisframework.md` als je de onderbouwing wilt lezen. Dat is geen stappenplan

## Volgende stappen

- [ ] Open beslissingen doorhakken, zie `05_bedrijf/framework/open-beslissingen.md`
- [ ] Twee casusklanten kiezen
- [ ] Eerste klantskills in `04_bibliotheek/skills/`, na de eerste klant. Zie de twee categorieën in `04_bibliotheek/README.md`
- [ ] Vóór/ná-demo bouwen als bewijsmiddel
- [ ] Proefopstelling lokale AI inplannen
