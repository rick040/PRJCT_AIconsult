# Operations: mailtriage [CONCEPT]

**Eigenaar:** `[naam bij de klant]` · **Laatst bijgewerkt:** 2026-08-25 · **Getest op:** 0 echte gevallen

> Concept. Nog niet bij een klant ingezet.

## Wat dit doet
Neemt een volle inbox door en levert per bericht: waar het over gaat, wie het moet oppakken, hoe urgent het is, en een conceptantwoord voor de berichten die standaard zijn.

## Wanneer gebruik je dit
- Aan het begin van de dag op de gedeelde inbox: info@, planning@, verkoop@
- Na een vakantie of een lange werkdag buiten kantoor
- Bij een piek na een storing, een mailing of een leveringsprobleem

## Wanneer juist niet
- Op persoonlijke mailboxen. Doe dit alleen op gedeelde inboxen met vastgelegde routering
- Bij juridische, arbeidsrechtelijke of klachtgevoelige berichten. Die gaan altijd handmatig
- Als er nog geen afspraak is over wie waarvan eigenaar is. Zonder dat raadt de skill

## Wat heb je nodig
- Toegang tot de gedeelde inbox, via de koppeling uit laag 3
- `00_bedrijf/procedures.md` met wie waarvan eigenaar is
- `00_bedrijf/spelregels-ai.md`: welke berichten nooit door AI gaan
- Vijf voorbeelden van standaardantwoorden zoals jullie ze schrijven

## Stappen
1. Lees de berichten van de afgelopen periode
2. Deel in: actie nodig, ter info, standaardantwoord, of niet door AI behandelen
3. Wijs per bericht een eigenaar toe op basis van `procedures.md`. Onduidelijk: markeer als "eigenaar onbekend", niet gokken
4. Bepaal urgentie op drie niveaus: vandaag, deze week, kan wachten
5. Schrijf een conceptantwoord voor alles in de categorie standaardantwoord
6. Zet de rest op een lijst met één regel per bericht
7. Meld apart wat je bewust hebt overgeslagen en waarom

## Wat komt eruit
Een overzicht, bijvoorbeeld:

```
Vandaag (4)
- Van Dijk BV, levering te laat. Eigenaar: planning. Concept klaar
- Sollicitatie monteur. Eigenaar: HR. Niet door AI behandeld

Deze week (9)
...

Overgeslagen (2)
- Klacht over factuur, valt onder spelregels-ai punt 3
```

## Wat kan er misgaan

| Wat je ziet | Wat er aan de hand is | Wat je doet |
|---|---|---|
| Veel "eigenaar onbekend" | Laag 0 is niet af: eigenaarschap ligt niet vast | Terug naar het structuurplan. Dit is de belangrijkste uitkomst van deze skill |
| Conceptantwoorden voelen te stijf of te los | Te weinig echte voorbeelden meegegeven | Vijf echte antwoorden toevoegen, opnieuw draaien |
| Iets gevoeligs krijgt toch een concept | `spelregels-ai.md` is te vaag | Categorieën scherper opschrijven, met voorbeelden |
| Urgentie klopt niet met hoe jullie werken | Urgentie is nergens gedefinieerd | Drie niveaus vastleggen in `procedures.md` |

## Altijd zelf controleren
Elk antwoord voordat het verstuurd wordt. Deze skill verstuurt nooit zelf.
