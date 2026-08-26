# n8n: workflowpatronen

Per patroon één bestand: welk probleem het oplost, hoe de flow loopt, waar hij stukgaat en hoe de klant hem zelf kan aanpassen.

**Nog leeg.** Er is nog geen workflow bij een klant opgeleverd.

## Verwachte volgorde van vullen

| # | Patroon | Waar het vandaan komt |
|---|---|---|
| 1 | Binnenkomende aanvraag naar dossier plus taak | Bijna elke intake noemt dit |
| 2 | Document naar de juiste map met de juiste naam | Dit is laag 0 die zichzelf onderhoudt |
| 3 | Inkoopfactuur naar controle en goedkeuring | Hoort bij `finance-factuurcontrole` |
| 4 | Terugkerende rapportage naar de directie | Levert het gesprek over de retainer op |

## Vaste opbouw per bestand

1. Welk probleem dit oplost, in de woorden van een klant
2. De flow in stappen, met bij elke stap wat er binnenkomt en wat eruit gaat
3. Waar handmatige goedkeuring in zit, en waarom daar
4. Wat er misgaat als een systeem eruit ligt, en wat de gebruiker dan ziet
5. Wat de klant zelf mag aanpassen en wat niet
6. Hoe je test dat hij nog werkt

## Regel over automatisering
Nooit een n8n-workflow bouwen voordat laag 0 en 1 staan. Een flow die documenten verplaatst in een mappenstructuur die nog gaat veranderen, is werk dat je twee keer doet. Zie `00_kern/lagenmodel.md`.

## Regel over stilte
Elke workflow meldt zichtbaar dat hij is gedraaid, ook als er niets te doen was. Een automatisering die zwijgt, wordt niet vertrouwd en na drie weken uitgezet.
