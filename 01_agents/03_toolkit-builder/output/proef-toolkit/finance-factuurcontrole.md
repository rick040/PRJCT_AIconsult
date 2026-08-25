# Finance: factuurcontrole [CONCEPT]

**Eigenaar:** `[naam bij de klant]` · **Laatst bijgewerkt:** 2026-08-25 · **Getest op:** 0 echte gevallen

> Concept. Nog niet bij een klant ingezet.

## Wat dit doet
Vergelijkt een inkoopfactuur met de bijbehorende opdracht of bestelling en meldt de verschillen, voordat er wordt goedgekeurd.

## Wanneer gebruik je dit
- Bij inkoopfacturen die aan een opdracht of bestelling gekoppeld zijn
- Bij terugkerende leveranciers waar de tarieven vastliggen
- Bij een stapel facturen na een drukke periode

## Wanneer juist niet
- Bij facturen zonder opdracht of bestelling erachter. Er is dan niets om mee te vergelijken
- Bij de eerste factuur van een nieuwe leverancier
- Als vervanging van de goedkeuring zelf. De skill controleert, een mens keurt goed

## Wat heb je nodig
- De factuur, digitaal
- De opdracht, bestelling of het contract
- `00_bedrijf/diensten-en-prijzen.md` of de afgesproken inkooptarieven
- De betalingstermijnen zoals jullie ze hebben afgesproken

## Stappen
1. Haal uit de factuur: leverancier, nummer, datum, regels, bedragen, btw, termijn
2. Zoek de bijbehorende opdracht of bestelling. Niet gevonden: stoppen en melden, niet doorwerken
3. Vergelijk regel voor regel: aantallen, tarieven, totaal, btw-tarief
4. Controleer de betalingstermijn tegen de afspraak
5. Maak een lijst met verschillen, met bij elk verschil het bedrag
6. Geef een conclusie in drie smaken: klopt, klopt met kleine afwijking, niet goedkeuren
7. Meld wat je niet hebt kunnen controleren

## Wat komt eruit
```
Leverancier: [naam]  Factuur: [nummer]  Bedrag: €[x]
Conclusie: niet goedkeuren

Verschillen:
- 12 uur gefactureerd, 8 uur op de opdracht. Verschil €[x]
- Btw 21%, op de opdracht 9%. Verschil €[x]

Niet kunnen controleren:
- Reiskosten, staan niet in de opdracht
```

## Wat kan er misgaan

| Wat je ziet | Wat er aan de hand is | Wat je doet |
|---|---|---|
| Opdracht wordt niet gevonden | Bestellingen worden niet vastgelegd, of niet vindbaar | Terug naar laag 0: waar leeft de bronwaarheid voor inkoop |
| Verschillen die geen verschil zijn | Afgesproken toeslagen staan nergens vast | Toeslagen en uitzonderingen vastleggen in de kennisbestanden |
| Bedragen worden verkeerd gelezen | Slecht gescande of fotografeerde facturen | Digitale facturen afdwingen bij de leverancier |
| Te veel wordt goedgekeurd | De skill is te soepel ingesteld | Drempel voor "kleine afwijking" expliciet in euro's vastleggen |

## Altijd zelf controleren
Elk bedrag en elke conclusie. Deze skill keurt niets goed en betaalt niets.
