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
