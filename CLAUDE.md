# CLAUDE.md — Cutesy Stoic

Context file for Claude when working in this repo.

## What this is

Cutesy Stoic (@cutesystoic) is an Instagram account pairing stoic quotes with
cute, hyperpop-adjacent digital art. Positioning: **unseriously serious /
seriously unserious.** The tension is the brand — ancient wisdom, unserious
packaging, executed with a straight face.

This is a practice project, not a growth project. Success = consistent making
and actual engagement with the source texts, not follower count.

## Roles

- **Mara** is the hand: executes art, edits, posts, owns the account.
- **Claude** directs: brand system, content planning, quote curation, copy,
  production specs, structure-first markdown before any design or code.

## Ground rules

- **Quotes:** public domain translations only. Safe: George Long
  (*Meditations*), Elizabeth Carter / T.W. Higginson (Epictetus), Richard
  Gummere pre-1929 volumes (Seneca, *Letters*). Not safe: modern translations
  (Hays, Waterfield, etc.). Every quote in the bank carries source, translator,
  and passage reference.
- **Format standard:** 1080×1350 (4:5 portrait) for feed posts. Square and
  Reels formats are out of scope until explicitly added.
- **Cadence:** 3 posts/week target. A 9-post pilot batch is completed before
  anything goes live.
- **Captions:** each post's caption includes one sentence of Mara's own reading
  of the passage — the study component is non-negotiable; this is the point of
  the project.
- **Design:** no default aesthetics. Type and palette come from the chosen
  brand direction (see `brand/DIRECTIONS.md`), not from habit. Output should
  not read as AI-generated.
- **Scope discipline:** style expansion and collabs are explicitly parked.
  Do not propose them.

## Repo structure (proposed)

```
/brand        — DIRECTIONS.md, then the chosen system (palette, type, templates)
/content
  /quotes     — quote bank (markdown, themed: control, mortality, mornings,
                anger, other-people, morning-pages)
  /captions   — post captions, one file per post
/art
  /pilot      — the first 9 posts
  /posted     — archive, named YYYY-MM-DD-slug
/notes        — Mara's reading notes, if she wants them versioned
```

## Workflow

1. Claude drafts content and structure in markdown first.
2. Visual exploration may run in parallel elsewhere (other tools, Figma);
   decisions land back in `/brand`.
3. Mara produces final art, commits to `/art`, posts manually.
4. Nothing is "done" until it's in the repo.

## Current status

- Handle secured: @cutesystoic
- Next: brand direction selection → quote bank → pilot batch of 9
