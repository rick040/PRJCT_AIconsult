# Bibliotheek

Herbruikbaar materiaal dat af is en bij meerdere klanten inzetbaar. Alles hier is ontdaan van klantdata.

| Map | Inhoud |
|---|---|
| `skills/` | skills per domein, plus het skill-sjabloon |
| `mcp/` | koppelingspatronen per systeem |
| `n8n/` | workflowpatronen |
| `fundament-sjablonen/` | domeinindelingen en mappenstructuren per branche |

## Twee soorten skills, twee verschillende regels

In `skills/` staan twee categorieën door elkaar. Ze zien er hetzelfde uit maar hebben een andere toelatingseis. Zet daarom bovenaan elke skill wie de eigenaar is, want dat bepaalt welke regel geldt.

### 1. Klantskills: eigenaar is de klant

Skills die we in een klanttoolkit opleveren. Voorbeelden: `sales-offerte-opstellen`, `operations-mailtriage`.

**Regel: die komen hier pas in als ze bij minimaal één klant hebben gewerkt én alle klantspecifieke gegevens eruit zijn.** Een idee hoort hier niet, een werkend patroon wel.

Concepten die daar nog niet aan voldoen, staan in `01_agents/03_toolkit-builder/output/proef-toolkit/` en verhuizen hierheen zodra ze zich hebben bewezen.

### 2. Werkwijzeskills: eigenaar is PRJCT AI

Skills waarmee onze eigen agents werken. Voorbeelden: `sales-koude-opvolging-cadans`, `scan-klantonderzoek-interviewgids`, `marketing-post-copywriting-checklist`, `marketing-landingspagina-cro-checklist`.

**Regel: die mogen hier meteen in, want er is geen klant om ze eerst bij te testen.** Ze beschrijven hoe wij werken, niet wat wij opleveren.

Wel geldt: zolang een werkwijzeskill nog niet in de praktijk is gebruikt, staat dat er eerlijk bij in het veld "Getest op". Niet leeg laten en niet mooier opschrijven dan het is.

## Waarom dit onderscheid bestaat

De oorspronkelijke regel ("pas hier in na één klant") is geschreven voor materiaal dat we aan klanten leveren. Voor onze eigen werkwijze slaat die eis nergens op: dan zou de bibliotheek pas gevuld raken nadat we onszelf aan een klant hadden verkocht. Zonder dit onderscheid spreken de twee categorieën elkaar tegen.
