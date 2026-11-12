# Feedback, round 5 (from Amélie, after reading checkpoint 5)

All three agents read this whole file. Rounds 1–4 still hold in full.

## The principle (standing, and the most important rule in this project)

**When Amélie names one instance, she is naming a class of failure.** When she asks "what are crossing links?", the
answer is not to fix that one phrase. It means: *this kind of thing failed*. Every instance of the class must be
found and fixed, everywhere in the paper, not only the one quoted.

So far we have fixed the quoted instances. That is not what was asked. From now on, every piece of feedback is
read as a class, and the fix is a search of the whole text for that class.

## What Amélie wants

A pedagogical paper:
- **no unnamed or unexplained objects**: every symbol, object, term and construction is named, defined before its
  first use, and explained (what it is, why it is there, the idea);
- **no redundancies**: each thing is said once, in the right place;
- **no jargon**: no word used to sound precise that a reader cannot understand from what came before;
- ideas first, then mathematics, with enumerated proof steps (rounds 2–4).

## Why self-checking was not enough

The symbol tables of round 3 and the rereads of round 4 were done by each author on their own text. An author
knows what their words mean, so they do not see what is unexplained. This round therefore uses **fresh eyes**:
each section is audited by an agent who did not write it.

## This round (round 6): cross-audit, then repair

### Phase A — audit (do not edit other agents' files)

| auditor | audits |
|---|---|
| dalmatian | Lattice fields, Local polynomials and activities (`part2/uv/01`, `02`) |
| greyhound | Infinite volume, Free Maxwell fields (`part2/limit/01`, `02`) |
| weimaraner | all of Part I and the Part II opening (`part1/*`, `part2/00-opening.tex`) |

Read the rendered PDF of your assigned sections **as a mathematician who has read only the earlier pages of the
paper**, slowly, line by line. Record **every** failure in `paper/audits/<auditor>-on-<owner>.md`, one numbered
finding per line: location (section, file and line), the exact words, the class of failure, and what is missing.
Classes:

- **U**: unexplained or unnamed object, symbol or term; used before it is defined; defined only inside a proof;
  defined but not explained;
- **R**: redundancy (said twice, a definition repeated, a paragraph that restates another);
- **J**: jargon (a word or phrase a reader cannot understand from what came before, including invented words);
- **D**: dense prose (a run of sentences where an enumeration or a display is needed; a proof idea not enumerated);
- **L**: a reference missing where an object is reused away from its definition.

Be exhaustive. Many findings is the expected result, not a failure. When the audit is complete, put
`AUDIT COMPLETE` as the last line of the file.

### Phase B — repair

When the audit of your sections is complete (check for the `AUDIT COMPLETE` line; `sleep 180` between checks):
1. Fix every finding.
2. **Generalise every finding.** For each one, ask what class it belongs to and search all of your text for other
   instances of that class (use `grep` for the words and patterns involved, and reread). Fix those too.
3. In `paper/audits/<owner>-response.md`, list for each finding what you changed, and for each class the further
   instances you found and fixed. Put `REPAIR COMPLETE` as the last line.

### Phase C — verification

When the owner's response file ends with `REPAIR COMPLETE`, the auditor rereads the repaired sections in the
rendered PDF and appends to its audit file: for each finding, `fixed` or `not fixed (why)`, and any new failures.
Last line: `VERIFIED`. The owner fixes anything marked not fixed.

### Then

Build, check the PDF, write `paper/reports/<name>-6.md` (at most one page: how many findings you raised and received,
by class; what remains), and **stop and wait**. No new sections this round. Once this method works, the remaining
sections will be written in the same way: drafted, cross-audited by another agent, repaired, verified.
