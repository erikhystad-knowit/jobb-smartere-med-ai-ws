# Jobb smartere med AI — personlig wiki

En personlig kunnskapsbase som bygges og vedlikeholdes av en LLM-agent, basert på
mønsteret beskrevet i [`llm-wiki.md`](llm-wiki.md).

Innretning: deltaker på Knowit Academy-kurset *"Jobb smartere med AI"*, med
**case-arbeid** som primær kilde — reelle arbeidsoppgaver hvor AI tas i bruk,
prøves ut, vurderes og reflekteres over.

## Hvordan det henger sammen

```
raw/        Dine kilder, uendret. Agenten leser herfra, men skriver aldri hit.
korpus/     Generert mellomlag for store caser: uttrukket tekst, manifest, triage.
wiki/       Agentens domene. Alle sider skrives og vedlikeholdes av agenten.
CLAUDE.md   Skjemaet. Forteller agenten hvordan wikien er bygd opp og hvordan den skal jobbe.
```

Du eier kildene og spørsmålene. Agenten gjør alt bokholderiet — sammendrag,
kryssreferanser, oppdatering av sider, indeks og logg.

## Kom i gang

1. **Legg en kilde i `raw/`** — notater fra et case, en oppgavebeskrivelse, et
   utklipp, en samtalelogg. Bilder og vedlegg i `raw/assets/`.
2. **Si fra til agenten:** *"les inn raw/\<filnavn\>"* eller *"her er et nytt case"*.
3. **Følg med.** Agenten diskuterer hovedpoengene med deg før den skriver, lager
   sidene, oppdaterer alt som berøres, og fører indeks og logg.

### Store caser (hundrevis av e-poster og dokumenter)

1. Legg materialet i `raw/caser/<kortnavn>/`.
   Mappestrukturen kan være som den kom. E-post: `.eml`, `.msg`, `.mbox` eller `.md` med `**Fra:**`-linjer.
   Dokumenter: `.pdf`, `.docx`, `.pptx`, `.xlsx`, `.csv`, `.txt`, `.md`, `.html`.
2. Si *"les inn caset <kortnavn>"*. Agenten kjører `uv run scripts/korpus.py inventar <kortnavn>`,
   som gir hvert element en fast ID (materialets egne, f.eks. `EM-001`, `FIN-003`, ellers `E-001`/`D-001`),
   trekker ut teksten og finner tråder.
3. Agenten spør hva oversikten skal brukes til og hvilke spørsmål den må svare på,
   triagerer alt i bolker, og skriver tema-, person- og dokumentsider i `wiki/caser/<kortnavn>/`.
   Start alltid med `wiki/caser/<kortnavn>/oversikt.md`.

Tre operasjoner:

| Si dette | Agenten gjør |
|---|---|
| *"les inn X"* / *"nytt case"* | Innlesing: leser kilden, skriver sider, oppdaterer alt som berøres |
| et spørsmål om materialet | Spørring: finner relevante sider, svarer med kildehenvisninger, tilbyr å arkivere svaret |
| *"lint"* / *"helsesjekk"* | Helsesjekk: motstrid, utdaterte påstander, foreldreløse sider, hull |

## Struktur i `wiki/`

| | |
|---|---|
| `index.md` | Katalog over alt. Leses først. |
| `log.md` | Kronologisk historikk. |
| `oversikt.md` | Den løpende syntesen — hva du mener nå. |
| `caser/` | Ett case per side — eller én mappe per stort case (oversikt, tema, personer, dokumenter, tidslinje, beslutninger). Kjernen. |
| `teknikker/` | Gjenbrukbare arbeidsmåter, utledet fra caser. |
| `verktoy/` | Verktøy og erfaringer med dem. |
| `innsikter/` | Svar og analyser som er verdt å beholde. |
| `kilder/` | Sammendrag av innleste kilder. |
| `maler/` | Maler å kopiere når nye sider lages. |

## Et par vaner som gjør wikien bedre

- **Gjengi prompter ordrett** i case-sidene. En omskrevet prompt er nesten
  verdiløs noen uker senere.
- **Skriv ned det som ikke fungerte.** Det er ofte mer nyttig enn det som gjorde det.
- **Seksjonen "Overførbart"** i hvert case er den som faktisk bygger kunnskap —
  det er derfra teknikkene kommer.
- **Arkiver gode svar.** Når du spør om noe og svaret er verdt å beholde, be
  agenten legge det i `innsikter/` i stedet for å la det forsvinne i chatten.
- Wikien er vanlige markdown-filer. Åpne mappa i **Obsidian** for å få
  wikilenker, grafvisning og søk.
