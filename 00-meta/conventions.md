# Vault Conventions

How this vault is organized and how to add to it.

## File and directory naming

- Directories are numbered to keep reading order: `01-foundation` … `13-characters`, with `00-meta` first and `99-reference` last.
- Character placement: the source bible's legendary empowered humans live in `05-empowered-humans/legendary-figures/`; all characters added since (contemporary cast, historical rulers, new legends of non-empowered people) live in `13-characters/`. The unified list is `12-indexes/characters.md`.
- Post-source additions carry `status: draft` and a `†` marker in index tables.
- Files are kebab-case: `the-hollow-king.md`, `iron-hand-marcus.md`.
- Every directory containing multiple entities has an `_index.md` listing its contents.
- One file per entity that is expected to grow (a god, a character, a glitch zone, a faction). Small related entries may share a category file (e.g. Class I Hollows) and can be promoted to their own file later — when promoting, leave a link behind in the category file.

## Frontmatter schema

Every content file opens with YAML frontmatter:

```yaml
---
title: Veranthos          # display name
type: deity               # deity | character | location | faction | creature | concept | event | artifact | index
category: the-twelve      # subgroup within the type (optional)
secrecy: public           # see secrecy tiers below
status: canon             # canon | draft | stub
---
```

Optional fields as relevant: `aka` (epithet/aliases), `alignment` (power affiliation),
`era` (timeline placement), `affinity` (Fluxborn element), `threat` (Hollow class or
zone threat level), `population`.

- `status: canon` — established in the source bible.
- `status: draft` — new material not yet locked in.
- `status: stub` — a known thin spot; the source gave only a line or two. Search for `status: stub` to find expansion targets.

## Secrecy tiers

The setting is built on layered hidden truths. Tag every file with the tier of its
most sensitive content:

| Tier | Meaning |
|---|---|
| `public` | Common in-world knowledge. Safe to show players/readers. |
| `restricted` | Known in-world only to elites — the Twelve, the Cabal, scholars. Revealing it is a plot event. |
| `gm-only` | Known to no one in-world (or only the Entity). The Entity, ARIA's full history, the Shriven, the Lunar Complex expansion. |

Files that are mostly public but contain a secret section keep the *file* at the
lower tier and mark the section heading, e.g. `## Secret (restricted)`.

## Linking

- Use relative markdown links: `[Kythera](../04-divine-beings/the-twelve/kythera.md)`.
- When two entities are connected (patron god ↔ noble house, city ↔ resident), link **both ways**.
- New named entities must be added to the matching cross-index in `12-indexes/`.

## Adding a new entity

1. Copy the matching template from `00-meta/templates/`.
2. Fill in frontmatter and whatever sections you have; delete sections you don't. Set `status: draft`.
3. Save it in the matching numbered directory.
4. Add it to that directory's `_index.md` and to the relevant `12-indexes/` file(s).
5. If it contradicts existing canon, either resolve it or record the conflict in [continuity-notes.md](continuity-notes.md).

## Dates

Year Zero is the Concordance (~2,100 years before present). Prefer relative dating
as the source does ("~800 years ago") until an in-world calendar is formalized —
that's an open worldbuilding task, see [continuity-notes.md](continuity-notes.md).
