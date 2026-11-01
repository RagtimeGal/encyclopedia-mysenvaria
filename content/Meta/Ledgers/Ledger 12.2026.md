---
title: "Lore Ledger 12.26"
enableToc: true
tags:
  - topic/meta/ledger
type: ledger
ledger_data:
  week: 12
  year: 2026
---

> [!abstract|callout-meta-general] [[Meta/Meta|Meta]] || Fourth Wall Ahead!
> The following article is metatextual. It provides information on what the *Encyclopedia Mysenvaria* is, how it should be used, how you can use it, and how you can help improve it.

> [!example|callout-ledger] [[Meta/Meta|Meta]] || Lore Ledger #15!
> This article serves as a brief changelog and project update announcement for the *Mysenvaria*.
>
> ... [[Meta/Ledgers/Ledger 10.2026|Lore Ledger 10.26]], **Lore Ledger 12.26**, [[Meta/Ledgers/Ledger 36.2026|Lore Ledger 36.26]] ...

This week pretty much every article across the entire Encyclopedia has been edited in some way.

Importantly, there's been a major refactor to the way the Encyclopedia's programs run. There is now one program which consolidates all YAML across the entire encyclopedia into one JSON file which is then used by other programs. This way programs do not each individually have to index the entire Encyclopedia and it is performed by one program which the others then use the labor of. This should theoretically massively speed up the Encyclopedia's programs.

This change actually occurred as I was attempting to find a way to combine all of the God biography pages while maintaining indexes like the List of Elemental Gods. This has introduced a new metadata key, `subpage`, which 'tricks' the programs into thinking pages which do not exist do exist, and thus links to them in indexes.

For the sake of my own sanity I will not be including a changed files table in today's ledger. There have been major textual edits, removals, and additions to metaphysics-related pages.
