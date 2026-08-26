# Workflow: Offerteaanvraag naar conceptofferte [MOCK, voorbeelduitvoer]

**Klant:** Van Hoof Installaties · **Domein:** Sales · **Datum:** 2026-11-09

> Voorbeelduitvoer van de integratie-agent, laag 3, bovenop de toolkit uit fase 2. Illustratief, geen werkende koppeling.

## Doel
Een binnenkomende offerteaanvraag via het contactformulier automatisch in de juiste klantmap zetten en de skill `sales-offerte-opstellen.md` klaarzetten, zodat Wendy niet meer handmatig hoeft over te typen. Scheelt circa 1,5 uur per week (use-case 3 uit het scanrapport).

## Trigger

| | |
|---|---|
| Type | webhook |
| Bron | Contactformulier op de website van Van Hoof |
| Frequentie | Bij elke nieuwe inzending |

## Nodes

| # | Node | Type | Wat het doet | Condities |
|---|---|---|---|---|
| 1 | Formulier ontvangen | Webhook | Vangt de inzending op (naam, adres, dienst, bericht) | n.v.t. |
| 2 | Klantmap controleren | Function | Zoekt of `01_klanten/[Klantnaam]/` al bestaat | Bestaat niet → aanmaken |
| 3 | Aanvraag wegschrijven | Move/Write | Zet de aanvraag als bestand in `01_klanten/[Klantnaam]/01_offertes/` | n.v.t. |
| 4 | Melding naar Wendy | Mail/Teams | Stuurt bericht: nieuwe aanvraag klaar voor de skill sales-offerte-opstellen | Alleen tijdens werkdagen 07:00-18:00, anders volgende werkdag |

## Verwachte uitkomst
Een nieuw bestand in de klantmap met de ruwe aanvraag, plus een melding aan Wendy dat er een conceptofferte kan worden opgesteld. Wendy start daarna zelf de skill.

## Foutafhandeling

| Wat gaat mis | Wat gebeurt er dan | Wie krijgt bericht |
|---|---|---|
| Website/formulier niet bereikbaar | Workflow slaat over, geen aanvraag verloren want formulier bewaart lokaal | Wendy, via foutmelding volgende ochtend |
| Verplicht veld leeg (bijvoorbeeld geen adres) | Aanvraag wordt toch weggeschreven, met markering "onvolledig" | Wendy, met verzoek om aan te vullen |
| Dubbele inzending (klant verstuurt formulier twee keer) | Tweede inzending wordt herkend op naam + tijdstip en samengevoegd | Geen apart bericht, samengevoegd zichtbaar in de map |

## Datagrenzen
Getoetst aan `spelregels-ai.md`: ja. Klantgegevens blijven binnen de eigen mapstructuur, gaan niet naar een externe chatbot.

## Beheer

| | |
|---|---|
| Interne beheerder | Wendy Smulders |
| Aan/uit zetten | Via de n8n-omgeving, knop "actief/inactief" op de workflow |
| Laatst getest | 2026-11-09, met drie praktijkgevallen inclusief een onvolledige aanvraag |
