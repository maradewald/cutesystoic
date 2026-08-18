# History

A decision log. Why things were built the way they were — not what changed.

## 2026-08-17 — Quote bank verified against public-domain sources

**What:** Ran the full verification pass on `content/quotes/QUOTES.md`. All 43
drafted quotes were checked against the actual translator texts; 11 wordings
corrected, 1 reference corrected, 1 entry cut as apocryphal.

**Why:** The bank's own rule is that every line must be the public-domain
translator's wording, not a paraphrase. Spot-checking would have missed the
real failure mode: several entries were *modern* translations wearing a
public-domain credit (notably Med. 4.3 and Ench. 1), which is the exact
copyright exposure the rule exists to prevent. "Control" instead of Carter's
"power" turned out to be a reliable tell.

**Alternatives considered:** Verifying by reading the texts by eye. Rejected —
the discrepancies that matter are single words ("this thing," "busybody,"
"leisure" vs "idleness"), so quotes were diffed programmatically against
locally downloaded source texts instead.

**Follow-ups:** Two verified lines (37, 42) are weak as graphics now that
they carry the real wording; flagged in the bank rather than cut, since that
is a design call. See TODO.md.

## 2026-08-17 — Source-text edition traps recorded in the bank

**What:** `QUOTES.md` sourcing rules now name specific editions and the
lookalikes to avoid.

**Why:** Three of the obvious sources are the wrong translation despite
matching titles: Gutenberg #2680 (*Meditations*) is Casaubon 1634, not Long;
Gutenberg #45109 (*The Enchiridion*) is Higginson, not Carter; Gutenberg
#10661 is Long's Epictetus. Gummere's Seneca is not on Gutenberg at all and
has to come from Wikisource. Anyone re-verifying later would lose the same
hour rediscovering this.
