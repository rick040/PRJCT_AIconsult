# Sales — Offerte opstellen [MOCK, voorbeelduitvoer]

**Eigenaar:** Wendy Smulders · **Laatst bijgewerkt:** 2026-10-19 · **Getest op:** 3 echte aanvragen van Van Hoof Installaties

> Voorbeelduitvoer van de toolkit-builder-agent, gebouwd volgens `04_bibliotheek/skills/_SKILL-TEMPLATE.md`. Illustratief, geen echte klanttoolkit.

## Wat dit doet
Zet een binnengekomen offerteaanvraag om in een conceptofferte, met de actuele prijzen uit `00_bedrijf/diensten-en-prijzen.md`.

## Wanneer gebruik je dit
- Bij een nieuwe offerteaanvraag via mail, telefoon of het contactformulier

## Wanneer juist niet
- Bij maatwerk buiten de standaarddiensten, bijvoorbeeld een ongebruikelijke installatie. Dan stelt Bas de offerte zelf op.
- Bij een vervolgofferte op een lopend project. Gebruik dan de bestaande offerte als basis, niet deze skill.

## Wat heb je nodig
- De aanvraag (mail, notitie van het telefoongesprek, of het formulier)
- Naam en adres van de klant
- Gevraagde dienst of diensten

## Stappen
1. Lees de aanvraag en noteer welke dienst(en) gevraagd worden.
2. Zoek de bijbehorende prijzen op in `00_bedrijf/diensten-en-prijzen.md`. Staat een dienst er niet in, stop en meld dat aan Bas.
3. Stel de offerte op volgens het vaste format: aanleiding, werkzaamheden, prijs, planning, voorwaarden.
4. Zet de offerte in de klantmap: `01_klanten/[Klantnaam]/01_offertes/[Klant]_Offerte_[JJJJ-MM-DD].md`.
5. Meld aan Bas dat de conceptofferte klaarstaat ter controle.

## Wat komt eruit
Een conceptofferte in de klantmap, klaar voor controle. Voorbeeld van de kop:

> Offerte — Fam. Verhoeven, vervangen cv-ketel, Helmond. Datum 2026-10-19, geldig tot 2026-11-02.

## Wat kan er misgaan

| Wat je ziet | Wat er aan de hand is | Wat je doet |
|---|---|---|
| Dienst staat niet in de prijslijst | Prijslijst is niet compleet of het is maatwerk | Stop, meld het aan Bas, vul niet zelf een prijs in |
| Aanvraag is onduidelijk over de gevraagde dienst | Klant heeft vaag geformuleerd | Bel of mail de klant voor verduidelijking voordat je een offerte opstelt |
| Twee offertes voor dezelfde klant dezelfde dag | Mogelijk dubbele aanvraag | Controleer bij Bas of Wendy voordat je verstuurt |

## Altijd zelf controleren
Bedragen, naam en adres van de klant, en de geldigheidsdatum. AI maakt fouten die er goed uitzien.
