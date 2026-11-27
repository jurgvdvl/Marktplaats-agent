# marktplaats-verkoper

Een skill voor Claude die als persoonlijke verkoper op Marktplaats werkt. Je geeft een item door, Claude levert prijs met onderbouwing, een plakklare advertentie, de juiste instellingen en houdt je inbox bij. Jij plaatst en keurt goed.

## Wat het doet

- Prijsonderzoek op basis van nieuwprijs, actueel aanbod en de totale kopersprijs inclusief verzending en Kopersbescherming
- Titel, beschrijving, kenmerken, categorie en fotolijst
- Instellingen: prijstype, bieden vanaf, levering, pakketklasse, Direct Kopen, advertentievorm
- Het plaatsformulier voorbereiden in Chrome, tot vlak voor de knop Plaats je advertentie
- Inbox lezen, conceptantwoorden schrijven, biedingen beoordelen
- Onderhandelen met technieken uit Never Split the Difference (Voss), Thinking, Fast and Slow (Kahneman), Oversubscribed (Priestley) en The Catalyst (Berger), alleen eerlijk toegepast
- Berichten schrijven in een korte, vriendelijke stijl, met sjablonen voor antwoord, tegenbod, reserveren en afhakers
- Favorieten bekijken en opruimen
- Live advertenties bijwerken na jouw akkoord
- Banden en velgen: DOT-code, steekmaat, naafgat en ET
- Ritme als iets niet verkoopt

## Spelregels in de skill

- Jij plaatst de advertentie zelf. De gebruiksvoorwaarden van Marktplaats verbieden plaatsen via een geautomatiseerd systeem.
- Claude verstuurt, accepteert, wijzigt of verwijdert niets zonder jouw akkoord per actie.
- Geen wachtwoorden, bankgegevens of cookies.
- Geen links of QR-codes uit koperberichten openen.

## Installeren

Je hebt Claude met skills nodig. Voor de browserrecepten ook de Claude in Chrome-extensie.

1. Download of clone deze repo.
2. Kopieer de map `marktplaats-verkoper/` naar je skills-map:
   - Claude Code: `~/.claude/skills/` (alle projecten) of `.claude/skills/` (alleen dit project)
   - Claude.ai en Claude Desktop: zip de map `marktplaats-verkoper` en upload hem via Instellingen, Capabilities, Skills
3. Start een nieuw gesprek en zeg bijvoorbeeld: "Ik wil deze fiets verkopen op Marktplaats" met foto's erbij.

## Altijd actuele cijfers

De skill bevat geen vaste tarieven of prijsindicaties. Verzendkosten, categoriekosten, Kopersbescherming, schrootprijzen en prijzen van vergelijkbare advertenties zoekt Claude bij elke advertentie opnieuw op, in het plaatsformulier, op de hulppagina's van Marktplaats of via de zoek-API. Ook plaatsen, namen en categorie-id's staan niet vast in de skill: Claude leest ze uit het formulier. Daardoor werkt hij in elk land en elk jaar, zolang het platform vergelijkbaar werkt.

## MCP-servers

De skill bevat een overzicht van onofficiele Marktplaats MCP-servers. Er is geen officiele MCP. Die servers gebruiken niet-gedocumenteerde endpoints en kunnen stuk gaan. De skill werkt zonder MCP.

## Disclaimer

Dit project is onofficieel en niet verbonden aan Marktplaats, Adevinta of 2dehands. Gebruik is op eigen risico. Respecteer de gebruiksvoorwaarden van Marktplaats.

## Bijdragen

Issues en pull requests zijn welkom, vooral voor:
- bijgewerkte zoekroutes en browserrecepten
- aanvullende categorie-specifieke regels (zoals bij banden en velgen)
- veranderingen in de Marktplaats-interface waardoor een browserrecept niet meer klopt

Houd de skill vrij van persoonlijke gegevens: geen namen, adressen, advertentie-id's of koperberichten.

## Licentie

MIT, zie [LICENSE](LICENSE).
