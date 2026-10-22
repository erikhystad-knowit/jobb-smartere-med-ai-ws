---
title: Logg
type: oversikt
opprettet: 2026-10-22
oppdatert: 2026-10-22
tags: [meta]
---

# Logg

Append-only. Nyeste oppføring nederst. Prefikset `## [` er med vilje konsistent
slik at loggen kan leses med enkle verktøy:

```
grep "^## \[" wiki/log.md | tail -5
```

Typer: `ingest` · `case` · `query` · `innsikt` · `lint` · `skjema`

---

## [2026-10-22] skjema | Wiki opprettet
Struktur, skjema (`CLAUDE.md`) og maler satt opp etter mønsteret i `llm-wiki.md`.
Innretning: personlig kunnskapsbase for deltaker på Knowit Academy-kurset
"Jobb smartere med AI", med case-arbeid som primær kildetype.
Sider berørt: [[index]], [[oversikt]], [[maler/case]], [[maler/kilde]],
[[maler/teknikk]], [[maler/verktoy]], [[maler/innsikt]].

## [2026-10-22] skjema | Støtte for korpus-caser (hundrevis av e-poster og dokumenter)
Forberedt for et case med ca. 240 e-poster og 40 dokumenter, der selve oppgaven er
å få oversikt. Én `kilder/`-side per fil skalerer ikke, så store caser får nå:
`raw/caser/<slug>/` for råmaterialet, et generert mellomlag `korpus/<slug>/`
(manifest, uttrukket tekst, triage) via `scripts/korpus.py`, og en case-mappe
`wiki/caser/<slug>/` med oversikt, tema-, person- og dokumentsider, tidslinje,
beslutningslogg og spørsmålsside. Sitering med korpus-ID-er (`[E-042]`, `[D-007]`).
Ny innlesingsflyt i faser (inventar → formål → triage → syntese → tverrgående →
dekning → refleksjon), ny loggtype `korpus`. Små caser fungerer som før.
Sider berørt: [[index]], [[maler/korpus/oversikt]], [[maler/korpus/case]],
[[maler/korpus/tema]], [[maler/korpus/person]], [[maler/korpus/dokument]],
[[maler/korpus/sporsmal]], [[maler/korpus/tidslinje]], [[maler/korpus/beslutninger]].

## [2026-10-22] korpus | nordflow — fase 0: inventar
Indeksert `raw/assets/CaseCorpus/` med `uv run scripts/korpus.py inventar nordflow --raw raw/assets/CaseCorpus`.
240 e-poster (md, 40 tråder), 43 dokumenter (30 finnes i to formater, slått sammen til én ID; formatene ble sjekket mot hverandre, ingen avvik),
ca. 44 000 ord totalt, periode 2025-09-18 – 2026-09-17, ingen uttrekksfeil. Materialets egne ID-er (`EM-`, `BOARD-`, `FIN-` …) brukes.
Ikke indeksert: `raw/caser/Nordflow_Firmapresentasjon*.pdf` (bakgrunn, avklares). Neste: fase 1 (formål og styrende spørsmål).
Sider berørt: [[index]], [[caser/nordflow/oversikt]], [[caser/nordflow/case]].
