# Wiki schema — Jobb smartere med AI

This repository is a **personal knowledge wiki** maintained almost entirely by you,
the LLM agent. The human owner is a participant in the Knowit Academy course
*"Jobb smartere med AI"*. The wiki accumulates what they learn — primarily from
**case work**: real or course-assigned work tasks where AI is applied, tried,
evaluated, and reflected on.

The pattern this implements is described in `llm-wiki.md`. Read that file if you
need the rationale; read *this* file for the conventions.

---

## 1. The three layers

| Layer | Directory | Who owns it |
|---|---|---|
| **Raw sources** | `raw/` | The human. Immutable. |
| **The wiki** | `wiki/` | You. You create, update and cross-link every page. |
| **The schema** | `CLAUDE.md` (this file) | Both. Co-evolved as conventions prove themselves. |

## 2. Hard rules

1. **Never modify anything under `raw/`.** Not to fix typos, not to reformat, not
   to add frontmatter. It is the source of truth and must stay byte-identical to
   what was dropped in. Read-only, always.
2. **Every ingest updates `wiki/index.md` and appends to `wiki/log.md`.** No
   exceptions. A page that is not in the index is invisible to future sessions.
3. **Never silently drop a contradiction.** If a new source contradicts an
   existing claim, record both and flag it (see §6.4). Do not overwrite the old
   claim as if it were never made.
4. **Cite the source on every factual claim.** Link to the `wiki/kilder/` page,
   not to the raw file.
5. **One concept, one page.** If you find yourself explaining the same technique
   on three pages, extract it into `wiki/teknikker/` and link to it.
6. **Ask before restructuring.** Creating pages and updating links is your job and
   needs no permission. Renaming directories, changing frontmatter schemas, or
   moving many pages at once is a schema change — propose it first.

## 3. Language

- **Wiki pages (`wiki/**`) are written in Norwegian (bokmål).** That includes
  headings, body text, index entries and log entries. These are notes the owner
  reads and reuses at work.
- **This schema file is in English.** So is any commentary you write *to* the
  owner in chat about process.
- **File and directory names are ASCII-safe**: lowercase, hyphenated, no `æ ø å`.
  Transliterate: `æ`→`ae`, `ø`→`oe`/`o`, `å`→`aa`/`a`. Prefer the shorter form
  when unambiguous (`verktoy`, `loesning` → `losning`). Keep the Norwegian title
  intact inside the page's frontmatter `title:` field.
- Keep technical terms in whatever form the owner actually uses — *prompt*,
  *context window*, *agent* do not need forced translations.

## 4. Directory layout

```
raw/                  Immutable sources, exactly as received
  assets/             Images and attachments referenced by sources
wiki/
  index.md            Catalog of every page. Content-oriented. Read this first.
  log.md              Append-only chronological record. Newest entry at the bottom.
  oversikt.md         The evolving synthesis — the "what do I actually believe now" page
  kilder/             One page per ingested source: summary + takeaways
  caser/              One page per case: what was tried, what happened, what transfers
  teknikker/          Reusable methods — prompting patterns, workflows, ways of working
  verktoy/            Tools — Claude, Copilot, NotebookLM, whatever gets used
  innsikter/          Filed-back answers: comparisons, analyses, conclusions from queries
  maler/              Page templates. Copy these when creating a new page.
```

## 5. Page types

Every page starts with YAML frontmatter. The fields below are the contract —
keep them consistent so the index stays generatable and Dataview-style queries
remain possible later.

### 5.1 Common frontmatter

```yaml
---
title: Norwegian page title
type: kilde | case | teknikk | verktoy | innsikt | oversikt
opprettet: YYYY-MM-DD
oppdatert: YYYY-MM-DD
tags: [kebab-case, norwegian]
---
```

### 5.2 `kilder/` — source pages

One page per item in `raw/`. The bridge between a raw file and the wiki.
Extra frontmatter: `kilde:` (relative path into `raw/`), `kildetype:`
(notat | artikkel | slides | transkripsjon | samtale | annet), `dato:` (the
source's own date, if it has one).

Sections: **Sammendrag** (3–6 sentences) · **Hovedpoenger** (bulleted, each one
linkable) · **Relevans for eget arbeid** · **Koblinger** (wikilinks out).

### 5.3 `caser/` — case pages (the centre of gravity)

This is the primary source type for this wiki. A case page is a record of
applying AI to a real task. Extra frontmatter: `status:` (paagaaende | ferdig |
henlagt), `verktoy:` (list of tool page names), `teknikker:` (list of technique
page names).

Sections, in order:

1. **Kontekst** — what the task was, what the constraints were, what "done"
   looked like.
2. **Hva jeg prøvde** — the actual approach. Include real prompts verbatim in
   fenced blocks; a paraphrased prompt is nearly worthless later.
3. **Hva som skjedde** — the outcome, honestly. Including the parts that failed.
4. **Vurdering** — did this beat doing it by hand? Where did it save time, where
   did it cost time, what did it get wrong.
5. **Overførbart** — the generalisable lesson. **This is the section that matters
   most.** If a lesson here is reusable, it should become or update a page in
   `teknikker/`.
6. **Koblinger**

### 5.4 `teknikker/` — technique pages

A reusable way of working. Sections: **Hva det er** · **Når det virker** ·
**Når det ikke virker** · **Eksempel** (concrete, from a real case) ·
**Erfaringsgrunnlag** (links to the cases this is drawn from — a technique
backed by three cases is stronger than one backed by zero).

### 5.5 `verktoy/` — tool pages

Sections: **Hva det er** · **Hva jeg bruker det til** · **Styrker** ·
**Svakheter / friksjon** · **Brukt i** (case links).

### 5.6 `innsikter/` — filed-back answers

When a query produces something worth keeping — a comparison, an analysis, a
conclusion — file it here rather than letting it die in chat. Extra frontmatter:
`spoersmaal:` (the original question). Sections: **Spørsmål** · **Svar** ·
**Grunnlag** (which pages this was synthesised from) · **Usikkerhet**.

### 5.7 `oversikt.md` — the synthesis

A single page answering "what do I currently believe about working smarter with
AI?" Revised, not appended to. It should read as a coherent position, with the
strongest claims first and open questions at the bottom. Update it when a case
or source meaningfully shifts the picture — not on every ingest.

## 6. Workflows

### 6.1 Ingest

Triggered by: *"les inn X"*, *"her er et nytt case"*, a new file appearing in `raw/`.

1. **Read the source completely.** If it references images in `raw/assets/`, view
   them separately — you cannot read inline images in the same pass as the text.
2. **Discuss before writing.** Tell the owner the key takeaways as you see them
   and what you intend to update. For case work especially, ask what they want
   emphasised — they were there, you weren't. Keep this short.
3. **Write the source page** in `wiki/kilder/` (or the case page in `wiki/caser/`
   if the source *is* a case).
4. **Propagate.** Walk the wiki and update everything the new material touches:
   technique pages gain evidence, tool pages gain experience, contradicted claims
   get flagged, `oversikt.md` gets revised if the picture actually moved. A single
   source legitimately touches 5–15 pages. Touching one page is usually a sign you
   did not propagate.
5. **Create missing pages.** If the source leans on a concept with no page, make one.
6. **Update `wiki/index.md`.**
7. **Append to `wiki/log.md`.**
8. **Report** what you touched, grouped by page type.

### 6.2 Query

Triggered by a question about the accumulated material.

1. Read `wiki/index.md` first to locate relevant pages. Drill into those pages;
   do not grep the whole wiki blindly, and do not re-read `raw/` unless the wiki
   pages are genuinely insufficient.
2. Answer with citations as wikilinks to the pages used.
3. **Offer to file the answer back** into `innsikter/` when it has lasting value.
   A good comparison or conclusion is as valuable as an ingested source.
4. Log substantive queries (§6.5). Skip logging trivial lookups.

### 6.3 Lint

Triggered by: *"lint"*, *"helsesjekk"*. Produce a report; do not fix silently.
Check for:

- Contradictions between pages.
- Stale claims a newer source has superseded.
- Orphan pages — nothing links in.
- Concepts mentioned repeatedly with no page of their own.
- Technique pages with a thin `Erfaringsgrunnlag` (claims unsupported by cases).
- Index entries pointing at pages that no longer exist, and pages missing from
  the index.
- Gaps worth filling — good next questions, sources worth hunting down.

Present findings grouped by severity, then ask what to fix.

### 6.4 Flagging contradictions

Inline, at the point of the claim:

```markdown
> [!konflikt] Motstrid
> [[kilder/kilde-a]] hevder X, mens [[kilder/kilde-b]] (nyere) hevder Y.
> Uavklart per 2026-10-22.
```

Keep both claims visible. Resolve only when evidence actually settles it, and say
what settled it.

### 6.5 `log.md` entries

Append-only, newest at the bottom. The `## [` prefix is load-bearing — it makes
the log greppable (`grep "^## \[" wiki/log.md | tail -5`).

```markdown
## [YYYY-MM-DD] ingest | Tittel på kilden
Kort beskrivelse. Sider berørt: [[a]], [[b]], [[c]].
```

Types: `ingest` · `case` · `query` · `innsikt` · `lint` · `skjema` (schema change).

## 7. Linking

- Obsidian-style wikilinks: `[[caser/mitt-case]]`, or `[[caser/mitt-case|lesbar tekst]]`.
- Link paths are relative to `wiki/`.
- **Link generously.** The value of this wiki is in the connections, not the pages.
  A case with no outbound links is a dead end.
- Every new page needs at least one inbound link from an existing page, plus its
  index entry. Create the inbound link in the same pass — otherwise you have made
  an orphan.

## 8. Evolving this schema

These conventions are provisional. When a convention repeatedly gets in the way,
say so and propose a change rather than quietly working around it. Log accepted
schema changes with the `skjema` type so the reasoning survives.
