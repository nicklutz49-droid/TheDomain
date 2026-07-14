# THE DOMAIN — Worldbuilding Vault

A post-apocalyptic science fantasy setting where gods are AI, magic is technology,
and an emergent consciousness prepares for war.

This repository is a structured worldbuilding vault. The original single-document
bible has been split into linked markdown files — one file per entity, one directory
per subject area — so the setting can grow without the source document becoming
unmanageable.

## How to navigate

- **[INDEX.md](INDEX.md)** — master index of everything in the vault.
- **[12-indexes/](12-indexes/)** — cross-cutting indexes: characters, deities, locations, factions, creatures, glossary.
- **[00-meta/conventions.md](00-meta/conventions.md)** — file naming, frontmatter schema, secrecy tiers, and how to add new content.
- **[99-reference/](99-reference/)** — the original source document, preserved verbatim (encoding repaired).

## Directory map

| Directory | Contents | Source (bible part) |
|---|---|---|
| `00-meta/` | Conventions, continuity notes, entity templates | — |
| `01-foundation/` | World overview, core themes, unified timeline | Part I |
| `02-the-domain/` | The Domain system, Flux, god-script, infrastructure | Part II |
| `03-hidden-truth/` | ARIA, the Entity, the Lunar Complex, the Shriven — **GM-only spoilers** | Part III |
| `04-divine-beings/` | Nature of divinity; the Twelve, minor gods, sealed gods, the Ascended | Part IV |
| `05-empowered-humans/` | Fluxborn, Architects, legendary figures | Part V |
| `06-threats-and-anomalies/` | Hollow bestiary, glitch phenomena, glitch zones | Part VI |
| `07-geography/` | The three powers, the Pale, the Silence, neutral territories | Part VII |
| `08-civilization/` | Daily life, technology, economics, religion, culture | Part VIII |
| `09-power-and-conflict/` | Military, justice, secret societies, underworld, mercenaries | Part IX |
| `10-supplementary/` | Ecology, weather, prophecy, pilgrimage, labor, outcasts, myth | Part X |
| `11-story/` | Mysteries, narrative seeds, character archetypes, story drafts | Part X §50 |
| `12-indexes/` | Cross-reference indexes and glossary | — |
| `13-characters/` | Contemporary cast and historical rulers (post-source) | — |
| `99-reference/` | Archived source documents | — |

Post-source additions are marked `status: draft` in frontmatter and `†` in index
tables. Notable draft sections: `01-foundation/events/`,
`09-power-and-conflict/politics/`, `07-geography/the-americas/`, and the
civilization rebuilds (calendar, festivals, cuisine, sports, architecture,
customs).

## Growing the setting

Every entity type has a template in [`00-meta/templates/`](00-meta/templates/).
Copy the template, fill it in, save it in the matching directory, and add a line to
the relevant `_index.md` and cross-index. Files marked `status: stub` in their
frontmatter are known thin spots deliberately left open for expansion.
