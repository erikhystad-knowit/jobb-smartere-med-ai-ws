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

## [2026-10-22] ingest | Nordflow – firmapresentasjon 2026
Leste inn `raw/caser/Nordflow_Firmapresentasjon.pdf` (2 sider; `(1)`-kopien er byte-identisk og ble ikke ført som egen kilde).
Brukes som bakgrunn til Nordflow-caset, ikke som del av korpuset. Re-kjørt inventar for `raw/assets/CaseCorpus/`: ingen nye filer (283 elementer, uendret).
Sider berørt: [[kilder/nordflow-firmapresentasjon]], [[caser/nordflow/oversikt]], [[index]].

## [2026-10-22] korpus | nordflow — skjelettsider
Opprettet `tidslinje`, `beslutninger`, `sporsmal` (tomme, fra malene) og genererte `katalog` slik at lenkene i casets oversikt løser seg innenfor `wiki/`. Fjernet en tom `caser/nordflow/tidslinje.md` i repo-roten som Obsidian hadde opprettet fra en uløst lenke.
Sider berørt: [[caser/nordflow/oversikt]], [[caser/nordflow/tidslinje]], [[caser/nordflow/beslutninger]], [[caser/nordflow/sporsmal]], [[caser/nordflow/katalog]].

## [2026-10-22] ingest | Nordflow – oppgavebeskrivelse
Leste `raw/caser/Nordflow-oppgave.pdf` (6 slides, tekstlaget ødelagt, lest som bilder). Oppgaven: 24-timers rådgivning til CEO før ekstraordinært styremøte,
fire mandatspørsmål, fem leveranser, vurderingskriterier. Dette besvarer fase 1 (formål og styrende spørsmål) for [[caser/nordflow/oversikt]].
Flagget motstrid i antall dokumenter/filer (40/315 i oppgaven mot 43/318 i inventaret) og en mulig dato-uoverensstemmelse (møte «torsdag» vs. «i morgen»).
Sider berørt: [[kilder/nordflow-oppgave]], [[caser/nordflow/oversikt]], [[caser/nordflow/case]], [[caser/nordflow/sporsmal]], [[index]].

## [2026-10-22] korpus | nordflow — mandatsider (parallelt utkast)
Fire sider, én per mandatspørsmål, skrevet parallelt av fire agenter rett fra korpuset (uten triage): [[caser/nordflow/mandat/01-hvor-star-oneflow]], [[caser/nordflow/mandat/02-hvorfor-havnet-vi-her]], [[caser/nordflow/mandat/03-hva-skjer-hvis-vi-ikke-handler]], [[caser/nordflow/mandat/04-hva-ma-besluttes-na]].
Kontroll: alle siterte ID-er finnes i manifestet (ingen ukjente), 161 av 283 elementer er sitert, nøkkeltall (395/472/506, 280, 146, 49 FTE m.fl.) er konsistente på tvers av sidene og stikkprøvekontrollert mot FIN-005, BOARD-004, HR-002, OPS-004, OPS-001, FIN-006, TECH-005, EM-173.
Sidene lister 9–10 motstrider hver (bl.a. 395 mot 472, sluttdato 28.2.2027 mot 30.6.2027, gul mot rød status, gevinst 184 mot 128). Triage (`triage.csv`) er ikke gjort. Skjemaendring: ny sidetype `mandat/` i korpus-case-mappa (`CLAUDE.md` §5.8).
Sider berørt: [[caser/nordflow/oversikt]], [[caser/nordflow/sporsmal]].
