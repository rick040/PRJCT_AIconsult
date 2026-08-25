# CLAUDE.md — werkinstructie voor elke agent in deze repo

Dit bestand wordt automatisch gelezen door Claude Code en Cowork. Lees het volledig voordat je iets doet.

## Wat deze repo is

Het werkbestand van **PRJCT AI**, de AI-implementatielijn van PRJCT Agency (Rick van Mierlo, Eindhoven/Geldrop). Doelgroep: MKB-bedrijven met 10-25 medewerkers in de Brainport-regio.

Deze repo is tegelijk het product. De structuur hier is dezelfde structuur die we bij klanten neerzetten. Behandel hem daarom als demonstratiemateriaal: als het hier rommelig wordt, verkopen we iets wat we zelf niet doen.

## Verplichte leesvolgorde

Voor elke opdracht, zonder uitzondering, eerst lezen:

1. `00_kern/positionering.md` — wie we zijn, wat we wel en niet doen
2. `00_kern/lagenmodel.md` — de inhoudelijke kern van de aanpak
3. `00_kern/prijskaart.md` — bij alles wat met geld te maken heeft
4. `00_kern/personas.md` — bij alles wat richting een klant gaat
5. `00_kern/tone-of-voice.md` — bij elke tekst

Daarna het `AGENT.md` van de agent waarin je werkt.

**Nooit een prijs, belofte of positioneringszin verzinnen die niet in `00_kern/` staat.** Staat het er niet in? Dan meld je dat en vraag je het, of je zet het als `[TE BEPALEN: ...]` in de output. Niet invullen op gevoel.

## Waar output landt

| Soort werk | Locatie |
|---|---|
| Klantspecifiek | `02_klanten/[Klant]/` — kopie van `_TEMPLATE/` |
| Generiek werkmateriaal, niet klantgebonden | `01_agents/[agent]/output/` |
| Herbruikbaar, af, voor meerdere klanten | `04_bibliotheek/` |
| Bedrijfsvoering PRJCT AI zelf | `05_bedrijf/` |

**Naamgeving:** `[Klant]_[Type]_[JJJJ-MM-DD].[ext]`
Voorbeeld: `DeGroot_Offerte_2026-09-14.pdf`

Varianten krijgen een eigen bestand met suffix `_v2`, `_v3`. Nooit overschrijven. Verouderd materiaal gaat naar `99_archief/`, wordt niet verwijderd.

## Werkregels

1. Nederlands, tenzij het bestand zelf Engels is.
2. Geen em-dashes gebruiken in output.
3. Direct en concreet. Geen inleidende beleefdheden, geen samenvattende afsluiting.
4. Bedragen altijd met euroteken en punt als duizendtalscheiding: €3.500.
5. Bij twijfel over scope: één vraag stellen, niet vijf.
6. Nooit klantdata uit `02_klanten/` in generieke bestanden of voorbeelden plakken.
7. Elke agent schrijft alleen in zijn eigen map en in `02_klanten/`. Wil je iets in `00_kern/` wijzigen, meld het en wacht op akkoord. Die bestanden zijn de bron van waarheid.

## Status van deze repo

Fase: opbouw. Veel bestanden zijn mock of skelet, herkenbaar aan `[MOCK]` in de titel of `[TE BEPALEN: ...]` in de tekst. Die zijn bedoeld om te vervangen door echt materiaal zodra dat er is. Behandel mock-inhoud nooit als feit richting een klant.
