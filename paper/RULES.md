# The rules of this paper

This file collects every standing rule from Amélie's feedback (`feedback/round-1.md` … `round-6.md`). It is the
checklist every section is written against and audited against. **Stick to it brutally.** When in doubt, the
feedback files give the examples; this file gives the rules.

## A. The governing principle

A0. **A named instance is a class of failure.** When Amélie (or an auditor) names one passage, find and fix every
    instance of that kind of failure everywhere in your text, not only the one quoted.

## B. The reader

B1. The reader is a human mathematician who wants to understand. Write for them, not to sound precise.
B2. **Every object, symbol and technical term is named, defined before its first use, and explained**: what it is,
    in which context, and what the idea is. No unnamed or unexplained objects.
B3. Objects used in more than one place have a displayed definition, never one buried in a proof.
B4. When an object is reused away from its definition, give a link (`\ref`, `\eqref`) to the definition, unless it
    is obvious from the immediate context.
B5. **No jargon.** No coined words; no word a reader cannot understand from what came before. Prefer plain
    mathematics or standard terms of the literature (constructive QFT, lattice gauge theory, Osterwalder–Schrader,
    Wightman, Balaban), used exactly as the literature uses them.
B6. **No redundancy.** Say each thing once, in the right place. No repeated roadmaps, definitions or summaries.
B7. Do not mention working mechanics in the prose: no talk of "markers", "obligations", "deferred proofs", Lean
    names or the writing process. Lean names only in footnotes or correspondence tables.

## C. Structure and style

C1. Part I is the model of the style. Part I is "The main theorem", Part II is "The construction".
C2. **Every section opens with an outline**: what it does, why, what follows, how it is structured (see the model
    outline quoted in `feedback/round-3.md` §3), with concrete references, not vague phrases.
C3. **Before each result, explain in words what it says and why it matters; then state it in short, precise
    mathematics.** Statements are clean: formulas or a short labelled list, not prose lists of properties.
C4. **Ideas first, then mathematics.** Every proof longer than a few lines starts with its idea in plain words.
    Technicalities go inside proofs, written as mathematics (displays), not as runs of sentences.
C5. **Use mathematics to express ideas**: a short display for each key step is clearer than a sentence.
C6. **Proof steps** (see `feedback/round-6.md`): a long proof is structured into steps written as
    `\medskip\noindent\textit{Step~1: Short description of the idea of the step.}` followed by the step's text and
    displays (use the `\proofstep` macro of `macros.tex`, which produces exactly this). Steps structure a long proof;
    each step is a substantial piece of argument, never a single sentence. Short proofs have no steps.
C7. Write `\frac{a}{b}`, not `a/b`. Size delimiters to their contents (`\bigl(`, `\Bigl(`, `\left(` …).
C8. All labelled items (R1–R15, P1–P4, W0–W3, O1–O2, T1–T4, Reg1–Reg4 and the like) are hyperlinks, and so is every
    mention of them.
C9. Part II never redefines what Part I defines; it links to it.
C10. British spelling with *-ise* endings (normalise, renormalisation, centre, colour, behaviour).
C11. No `\clearpage` before sections (only between parts).

## D. Fidelity

D1. Claim nothing the Lean does not prove. Check every statement (hypotheses, quantifiers, order of choices, order of
    limits) against the pinned source at `/root/code/OpenAI-YM-20261028` (commit `3456e5e`).
D2. Never strengthen a statement for elegance. Where a proof is missing, leave a visible `\gap{...}` stating the
    missing mathematics plainly (no jargon inside the gap either).

## E. Process

E1. **Self-check before handing a section to its auditor**: reread your section in the rendered PDF against every
    rule in this file, rule by rule, and fix what fails. Record in your notes, per rule, what you checked and fixed.
E2. **Cross-audit**: every section is audited by an agent who did not write it (classes U, R, J, D, L of
    `feedback/round-5.md`, plus **S** for any violation of a rule in section C), repaired by its owner with the
    class-wide search of A0, and verified by the auditor.
E3. Edit only files you own. No subagents, ever. No commits, pushes or git configuration changes.
E4. Never leave the build broken.
